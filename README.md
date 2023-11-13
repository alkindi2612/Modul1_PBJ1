# Modul1_PBJ1

Created By Alkindi Syamsi 21343003

pada Pertemuan ini, kita hanya melakukan latihan dasar mengenai node.js yang pertama kita akan membuat script untuk menampilkan suatu tulisan

terdapat syntax console.log('Welcome to Node.js!!')
Potongan syntax berikut adalah potongan kode JavaScript menggunakan fungsi console.log() di Node.js. Ini mencetak pesan "Welcome to Node.js!!" ke konsol. Fungsi console.log() umumnya digunakan untuk debugging dan menampilkan informasi di konsol. Pada kasus ini, itu mencetak pesan yang ditentukan.

lalu kita diminta membuat sebuah file/program baru yang nanti nya akan ditampikan pada halaman browser
Berikut penjelasan singkatnya:

1. Import Modul HTTP:
   const http = require('http');
   Mengimpor modul HTTP yang sudah tersedia di Node.js.

2. Konfigurasi Host dan Port:
   const hostname = '127.0.0.1';
   const port = 2612;
   Menentukan alamat host dan nomor port server.

3. Membuat Server:
   const server = http.createServer((req, res) => {
       // Pengaturan respons
       res.statusCode = 200;
       res.setHeader('Content-Type', 'text/plain');
       res.end('Hello KINNN\n');
   });
   Membuat server HTTP yang akan merespons dengan pesan "Hello KINNN" jika diakses.

4. Menjalankan Server:
   server.listen(port, hostname, () => {
       console.log(`Server running at http://${hostname}:${port}/`);
   });
   Menjalankan server pada host dan port yang telah ditentukan, dan mencetak pesan ke konsol saat server berjalan.
