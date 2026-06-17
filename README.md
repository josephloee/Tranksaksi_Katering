# Tranksaksi_Katering
plikasi berbasis web untuk layanan pemesanan katering secara online. Sistem ini dirancang untuk mempermudah proses interaksi antara pelanggan dan pengelola bisnis. Aplikasi ini terintegrasi dengan basis data relasional untuk mengelola katalog menu, informasi pengguna, dan riwayat transaksi secara terstruktur.

👥 Hak Akses Pengguna
Pembeli (Buyer): Pengguna yang mendaftar untuk melihat katalog menu, melakukan pemesanan untuk tanggal tertentu, memantau status pesanan, dan melihat riwayat transaksi mereka.

Admin: Pengelola sistem yang memiliki akses penuh untuk menambah atau mengubah katalog menu, mengelola data pelanggan, serta memverifikasi dan memperbarui status pesanan yang masuk.

🔄 Alur Proses Transaksi
>Eksplorasi Menu: Pembeli menelusuri pilihan paket katering dan menambahkannya ke keranjang pesanan.
>Checkout & Detail Pengiriman: Pembeli melengkapi formulir pemesanan, termasuk alamat pengiriman, tanggal, dan waktu acara.
>Proses Pembayaran: Sistem menerbitkan tagihan dengan status transaksi "Menunggu Pembayaran".
>Verifikasi Admin: Setelah pembeli melakukan pembayaran, Admin akan memverifikasi dana yang masuk dan memperbarui status transaksi menjadi "Diproses".
>Pengiriman & Selesai: Saat pesanan sedang diantar, status berubah menjadi "Dikirim", dan akan menjadi "Selesai" saat pesanan sudah diterima oleh pembeli.

🗄️ Gambaran Basis Data
>Tabel Pengguna (Users): Menyimpan kredensial login dan data profil, dilengkapi dengan kolom Role/Level untuk membedakan hak akses antara Admin dan Pembeli.
>Tabel Menu (Produk): Menyimpan informasi detail mengenai paket katering, termasuk nama, deskripsi, harga, dan ketersediaan.
>Tabel Transaksi (Orders): Mencatat informasi utama pesanan seperti ID Pembeli, tanggal pemesanan, tanggal acara, total harga, dan status pesanan.
>Tabel Detail Transaksi (Order Details): Terhubung dengan Tabel Transaksi untuk mencatat rincian spesifik (jumlah porsi dan jenis menu) yang dibeli dalam satu nomor pesanan.
