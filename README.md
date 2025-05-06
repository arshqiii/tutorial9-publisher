# Tutorial 9 - Software Architecture

## Muhammad Radhiya Arshq - 2306275885

### a. How much data your publisher program will send to the message broker in one run?
Dalam satu kali jalan jumlah data yang dikirim ke message broker oleh publisher adalah 5. Ini bisa dilihat dari kode main.rs pada fungsi main dipanggil method publish_event sebanyak 5 kali dengan data yang berbeda.  


### b. The url of: “amqp://guest:guest@localhost:5672” is the same as in the subscriber program, what does it mean?
Url yang dipakai program subscriber dan publisher sama karena keduanya terhubung ke server AMQP yang sama, bagian-bagian url tersebut sama artinya seperti yang di subscriber yaitu "guest" pertama merupakan username yang digunakan untuk login ke message broker, "guest" kedua merupakan password dari user guest, dan localhost:5672 merupakan alamat host server sekaligus port default untuk protokol AMQP yang digunakan message broker, dalam kasus ini, RabbitMQ.

### Running RabbitMQ as Message Broker
![alt text](image_1.png)