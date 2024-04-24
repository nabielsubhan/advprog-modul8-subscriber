## Nama   : Muhammad Nabiel Subhan
## NPM    : 2206081553
## Kelas  : AdPro B

### What is amqp
AMQP adalah singkata dari Advanced Message Queuing Protocol. AMQP berfungsi sebagai protokol standar untuk mengirim, menerima, dan mengelola pesan antar aplikasi yang terhubung dalam sebuah sistem. AMQP diimplementasikan pada arsitektur yang berorientasi pesan dimana komunikasi antar komponen terjadi melalui pertukaran pesan.

### What it means? guest:guest@localhost:5672 , what is the first quest, and what is the second guest, and what is localhost:5672 is for?  
Format tersebut adalah koneksi URL untuk melakukan koneksi dengan AMQP broker. Guest pertama menandakan `username`, sedangkan guest kedua adalah `password` dari username tersebut. "localhost:5672" merepresentasikan *hostname* (localhost) dimana AMQP broker berjalan dan nomor port (5672) untuk AMQP broker menerima koneksi.

### Simulation slow subscriber
<p align="center">
  <img src="images\simulation-slow-subscriber.png" />
</p>
Dapat dilihat bahwa terdapat 20 pesan pada message queue, karena terdapat buffer sehingga terdapat jeda 1 detik untuk proses pengiriman pesan. Hal ini terjadi ketika saya melakukan `cargo run` pada publisher sebanyak 5 kali.