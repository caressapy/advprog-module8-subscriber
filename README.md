# Subscriber App

## Reflection

Apa itu amqp?
AMQP adalah singkatan dari Advanced Message Queuing Protocol, yaitu sebuah protokol standar terbuka yang digunakan untuk komunikasi berbasis antrian pesan (message queue). Protokol ini memungkinkan berbagai aplikasi saling bertukar pesan secara andal, terstruktur, dan aman meskipun dijalankan secara terpisah atau dalam bahasa pemrograman yang berbeda. AMQP bekerja di lapisan aplikasi, mirip dengan protokol seperti HTTP, dan digunakan untuk memastikan bahwa pesan dikirim dan diterima dengan cara yang konsisten. Salah satu pola komunikasi yang didukung oleh AMQP adalah model publisher-subscriber, di mana pengirim (publisher) mengirim pesan dan penerima (subscriber) menerima pesan berdasarkan langganan terhadap topik tertentu. Dalam aplikasi ini, protokol AMQP dimanfaatkan untuk menghubungkan program publisher dan subscriber melalui message broker seperti RabbitMQ.

Apa maksud dari "guest:guest@localhost:5672"?
Alamat "guest:guest@localhost:5672" adalah bagian dari URI koneksi yang digunakan untuk mengakses server AMQP, seperti RabbitMQ. Format ini berisi informasi autentikasi serta alamat server dan port yang digunakan. guest adalah username default yang disediakan oleh RabbitMQ, dan guest yang kedua adalah password-nya. localhost menunjukkan bahwa aplikasi akan terhubung ke server RabbitMQ yang berjalan di komputer lokal. Sedangkan 5672 adalah port default yang digunakan oleh protokol AMQP untuk menerima koneksi. Jadi, URI ini secara lengkap menunjukkan bahwa aplikasi akan terhubung ke broker lokal dengan kredensial default pada port standar.
