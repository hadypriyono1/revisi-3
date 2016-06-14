# revisi-3
berikut mengenai node.js by ketua


Node.JS: pengertian, fungsi, dan aplikasi sederhana
Posted on September 27, 2015 by maqrikisandi	

Apa itu Node.JS?

Node.js adalah sebuah perangkat lunak yang didisain untuk mengembangkan aplikasi berbasis WEB. Node.js dieksekusi sebagai aplikasi server. Platform ini menggunakan bahasa pemrograman javascript dan menggunakan teknik non-bloking untuk mempercepat proses. Teknik non-bloking adalah sebuah metode penyelesaian sebuah fungsi.
Bahasanya baku amat ya’,😀
yup, karena itu salah satu paragraf yang ada di skripsi saya,😀

jadi node.js menurut kalimat diatas adalah sebuah platform yang menggunakan bahasa javascript untuk dieksekusi sebagai server. Biasanya kita mengenal aplikasi server itu pake bahasa PHP tapi kok ini javascript? itulah kelebihan node js, kita bisa menggunakan javascript yang dieksekusi sebagai server-side, kelebihan lain adalah teknik non-blocking yang ada di node.js, teknik non-blocking menurut yang dijelasin di sini,  Teknik non-bloking yaitu teknik dimana node.js akan melakukan eksekusi secara independen. Node.js akan mengeksekusi sebuah operasi tanpa harus menunggu operasi sebelumnya selesai dieksekusi, sehingga menghasilkan aplikasi web yang lebih cepat dan efisien. Node.js dengan teknik non-bloking dapat diilustrasikan sebagai sebuah restoran, saat kita datang ke sebuah restoran, pelayan akan mencatat pesanan kita lalu menyerahkan pesanan ke petugas memasak, setelah itu pelayan akan mencatat pesanan orang lain lalu menyerahkan pesanan tersebut ke petugas memasak tanpa harus menunggu pesanan kita selesai dikerjakan dan begitu seterusnya hingga semua pesanan diantar ke pelanggan.

Oke, dari pada kita fusing-fusing pake kata-kata,kita coba buat sebuah aplikasi web hello-word pake node.js. pertama siapkan kopi dulu biar ga terlalu tegang,😀

instalasi node.js dan npm

    oke, pertama download node.js nya di sini, selesai download install seperti biasa, karena saya pake windows jadi tinggal klik next doang, selain windows saya belum bisa,😀
    selanjutnya adalah update npm. npm itu adalah package manager resmi untuk node.js, ibarat nya npm itu adalah tempat kita nyari dan download module-module yang kita butuhin untuk membangun sebuah aplikasi berbasis node.js
    untuk update nya pertama buka command prompt node.js, inget ya command prompt node js, bukan command prompt windows, setelah kebuka ketikkan perintah berikut:

        npm install npm -g

    biarin proses download nya kelar.

langkah selanjutnya yaitu membuat aplikasi hello-word pake node.js

    pertama kita bikin folder di document dengan nama cobaNodejs, nama folder ini terserah rekan-rekan semua:)
    terus buka command prompt node.js, terus kita arahkan lokasi direktorinya ke nama folder yang udah kita buat,
    setelah itu, kita download module expressnya dulu, module express ini berguna sebagai UI nya aplikasi node js (kalo salah mohon diingatkan karena itu pengertian yang saya tau :))
    cara download nya ketikkan perintah berikut:

        npm install express

    “npm install” itu adalah perintah default untuk download modul-modul node js, “express” sebagai modul yang kita download, tunggu instalasi kelar,
    langkah selanjutnya buka IDE javascript, bisa pake nodepad++, nodepad, sublime, aptana, dll
    terus ketikkan kode seperti dibawah ini

var express = require('express');
var app = express();

app.get('/', function (req, res) {
  res.send('Hello World!');
});

var server = app.listen(3000, function () {
  var host = server.address().address;
  var port = server.address().port;

  console.log('Example app listening at http://%s:%s', host, port);
});

    setelah itu simpan di folder cobaNodejs dengan nama file cobaNodejs jangan lupa file extention nya javascript.:)
    setelah selesai disimpan, buka lagi command promp node.js,
    setelah command prompt node js nya kebuka kita menuju direktori yang ada file cobaNodejs tadi, terus ketikkan perintah berikut, lalu tekan enter

    node cobaNodejs.js

contohnya kayak gambar dibawah ini:

node js
