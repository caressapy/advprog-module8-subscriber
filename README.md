# Subscriber App

## Reflection

### Apa itu `amqp`?

`amqp` adalah singkatan dari **Advanced Message Queuing Protocol** — yaitu protokol komunikasi yang dirancang untuk mengatur pengiriman pesan antar layanan (*services*) dalam sebuah sistem. Protokol ini bekerja di lapisan aplikasi, seperti `HTTP` atau `HTTPS`, dan memungkinkan data (pesan) dikirim dalam bentuk *stream of bytes*.

Dalam konteks penggunaannya, `amqp` mendukung beberapa pola komunikasi, termasuk model **publisher-subscriber**, di mana satu pihak mengirimkan pesan dan pihak lain menerima berdasarkan langganan (*subscription*). Model inilah yang akan digunakan dalam aplikasi subscriber ini.

---

### Apa maksud dari `"guest:guest@localhost:5672"`?

URI ini adalah format standar untuk menyambung ke server `amqp`. Berikut penjelasannya:

* `guest`: username untuk mengakses broker AMQP.
* `guest`: password untuk username tersebut.
* `localhost`: berarti koneksi dilakukan ke server yang berjalan di mesin lokal (komputer sendiri).
* `5672`: port default yang digunakan oleh server AMQP (seperti RabbitMQ).

Jadi, `"guest:guest@localhost:5672"` berarti kita akan menghubungkan aplikasi subscriber ke server AMQP lokal, menggunakan kredensial username dan password `guest`, melalui port 5672.
