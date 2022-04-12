# Lab5Web
## Praktikum 5 : Java Script

## A. Langkah-Langkah Praktikum
Persiapan membuat dokumen HTML dengan nama file lab5_javascript.html seperti berikut.

`<!DOCTYPE html>`
<html lang="en">
`<head>`
`    <title>Mengenal JavaScript</title>`
`</head>`
`<body>`
    `<h1>Pengenalan Javascript</h1>`
    `<h3>Contoh document.write dan console.log</h3>`
    `<script>`
    `    document.write("Hello Word");`
    `    console.log("Hello Word");`
    `</script>`
`</body>`
`</html>`

![Gambar1](screenshot/ss1.png)

Tampilan contoh Javascript pada browser.

![Gambar2](screenshot/ss2.png)


## Javascript Dasar
## 1. Pemakaian Alert sebagai property window.
Selanjutnya kita akan menampilkan Alert box dengan Javascript. Masukan Kode seperti di bawah ini :

`<!DOCTYPE html>`
`<html lang="en">`
  `<head>`
    `<meta charset="UTF-8" />`
    `<meta http-equiv="X-UA-Compatible" content="IE=edge" />`
    `<meta name="viewport" content="width=device-width, initial-scale=1.0" />`
    `<title>Alert Box</title>`
  `</head>`
  `<body>`
    `<script lang="javascript">`
      
      window.alert("ini merupakan pesan untuk anda");
      
    `</script>`
  `</body>`
`</html>`

![Gambar3](screenshot/ss3.png)

Tampilan contoh Alert Box pada browser.

![Gambar4](screenshot/ss4.png)


## 2. Method dalam objek
Disini kita mencoba memakai javascript sebagai objek. Masukkan kode berikut :

`<!DOCTYPE html>`
`<html lang="en">`
`<head>`
  `<meta charset="UTF-8">`
  `<meta http-equiv="X-UA-Compatible" content="IE=edge">`
  `<meta name="viewport" content="width=device-width, initial-scale=1.0">`
  `<title>Script JavaScript</title>`
`</head>`
`<body>`
  Percobaan memakai javascript: `<br>`
  `<script lang="javascript">`
    
    document.write("Selamat Mencoba javascript<br>");
    document.write("Semoga Sukses !");
    
  `</script>`
`</body>`
`</html>`

![Gambar5](screenshot/ss5.png)

Tampilan contoh Method dalam objek pada browser.

![Gambar6](screenshot/ss6.png)


## 3. Prompt
Prompt digunakan untuk memasukkan data, bentuknya sama seperti alert box. kita masukkan kode berikut :

`<!DOCTYPE html>`
`<html lang="en">`
`<head>`
  `<meta charset="UTF-8">`
  `<meta http-equiv="X-UA-Compatible" content="IE=edge">`
  `<meta name="viewport" content="width=device-width, initial-scale=1.0">`
  `<title>Pemasukan Data</title>`
`</head>`
`<body>`
  `<script lang="javascript">`
    var nama=prompt("siapa nama Anda?","Masukkan nama anda");
    document.write("hai, "+ nama );
  `</script>`
`</body>`
`</html>`

![Gambar7](screenshot/ss7.png)

Tampilan contoh pada browser.

![Gambar8](screenshot/ss8.png)

jika kita ketik sebuah nama, maka akan muncul kalimat 'hai, (nama)'.


## 4. On load
sama seperti alert box, masukkan kode berikut :

`<!DOCTYPE html>`
`<html lang="en">`
  `<head>`
    `<title>Contoh program javascript</title>`
    `<script lang="javascript">`
      function pesan() {
        alert ("memanggil javascript lewat body onload")
      }
   `</script>`
  `</head>`
  `<body onload="pesan()">`
  `</body>`
`</html>`

![Gambar9](screenshot/ss9.png)

Tampilan hasil pada browser.

![Gambar10](screenshot/ss10.png)


## 5. Operasi Aritmatika
Operasi dasar aritmatika menggunakan JavaScript. Ketiklah kode berikut :

`<!DOCTYPE html>`
`<html lang="en">`
`<head>`
  `<meta charset="UTF-8">`
  `<meta http-equiv="X-UA-Compatible" content="IE=edge">`
  `<meta name="viewport" content="width=device-width, initial-scale=1.0">`
  `<title>Contoh Program Javascript</title>`
  `<script lang="javascript">`
    function test (val1,val2)
    {
      document.write("<br>"+"perkalian : val1*val2"+"<br>")
      document.write(val1*val2)
      document.write("<br>"+"pembagian : val1/val2"+"<br>")
      document.write(val1/val2)
      document.write("<br>"+"penjumlahan : val1+val2"+"<br>")
      document.write(val1+val2)
      document.write("<br>"+"pengurangan : val1-val2"+"<br>")
      document.write(val1-val2)
      document.write("<br>"+"modulus : val1%val2"+"<br>")
      document.write(val1%val2)

    }
  `</script>`
`</head>`
`<body>`
  `<input type="button" name="button1" value="arithmethic" onclick="test(9,4)">`
`</body>`
`</html>`

![Gambar11](screenshot/ss11.png)

Tampilan hasil pada browser.

![Gambar12](screenshot/ss12.png)

Jika kita klik tombol tersebut, maka akan muncul aritmatikanya.

![Gambar13](screenshot/ss13.png)


## 6. If - Else
Sekarang kita akan membuat program if else. Program yang dibuat pada Praktikum ini adalah nilai rendah dan tinggi. jika kita masukan nilai diatas 60, maka program akan menampilkan hasil 'lulus', Sebaliknya jika kita masukan nilai di bawah 60 maka program akan menampilkan hasil 'tidak lulus'. berikut kodenya :

`<!DOCTYPE html>`
`<html lang="en">`
`<head>`
  `<meta charset="UTF-8">`
  `<meta http-equiv="X-UA-Compatible" content="IE=edge">`
  `<meta name="viewport" content="width=device-width, initial-scale=1.0">`
  `<title>Contoh if-else</title>`
`</head>`
`<body>`
  `<script lang="javascript">`
    var nilai = prompt("nilai (0-100): ", 0);
    var hasil = "";
    if (nilai >= 60) 
    hasil = "Lulus";
    else
    hasil = "Tidak Lulus";
    document.write("hasil: " + hasil);
  `</script>`
`</body>`
`</html>`

![Gambar14](screenshot/ss14.png)

Tampilan hasil pada browser.

![Gambar15](screenshot/ss15.png)

Jika kita masukan nilai 60, maka akan muncul hasilnya keterangan hasil : Lulus.

![Gambar16](screenshot/ss16.png)


## 7. Operator Switch
Penggunaan operator switch untuk seleksi kondisi, Ketik kode berikut :

`<!DOCTYPE html>`
`<html lang="en">`
`<head>`
  `<meta charset="UTF-8">`
  `<meta http-equiv="X-UA-Compatible" content="IE=edge">`
  `<meta name="viewport" content="width=device-width, initial-scale=1.0">`
  `<title>Contoh program javascript</title>`

  `<script lang="javascript">`
    function test ()
    {
      val1=window.prompt("input nilai (1-5):")
      switch (val1)

      {
        case "1":
          document.write("bilangan satu")
          break
        case "2":
          document.write("bilangan dua")
          break
        case "3":
          document.write("bilangan tiga")
          break
        case "4":
          document.write("bilangan empat")
          break
        case "5":
          document.write("bilangan lima")
          break
        default :
          document.write("bilangan lainnya")
      }
    }
  `</script>`
`</head>`
`<body>`
  `<input type="button" name="button1" value="switch" onclick="test()">`
`</body>`
`</html>`

![Gambar17](screenshot/ss17.png)

Tampilan hasil pada browser.

![Gambar18](screenshot/ss18.png)

Jika kita klik tombol tersebut, maka akan muncul tampilan berikut, menunjukan bilangan yang kita pilih, yaitu angka 0-5.

![Gambar19](screenshot/ss19.png)

Jika yang kita masukan adalah bilangan yang lebih dari 5, maka akan menampikan hasil 'bilangan lainnya'.

![Gambar20](screenshot/ss20.png)


## 8. Form Input
Ketik kode seperti berikut.

`<!DOCTYPE html>`
`<html lang="en">`
`<head>`
  `<meta charset="UTF-8">`
  `<meta http-equiv="X-UA-Compatible" content="IE=edge">`
  `<meta name="viewport" content="width=device-width, initial-scale=1.0">`
  `<title>form input</title>`

  `<script lang="javascript">`
    function test (){
      var val1=document.kirim.T1.value
      if (val1%2==0)
        document.kirim.T2.value="bilangan genap"
      else 
        document.kirim.T2.value="bilangan ganjil"
    }
  `</script>`
`</head>`
`<body>`
  `<form method="post" name="kirim">`
    `<p>BIL <input type="text" name="T1" size="20"> MERUPAKAN BIL <input type="text" name="T2" size="20"></p>`
    `<p><input type="button" value="tebak" name="B1" onclick="test()"></p>`
  `</form>`
`</body>`
`</html>`

![Gambar21](screenshot/ss21.png)

Tampilan hasil pada browser.

![Gambar22](screenshot/ss22.png)


## 9. Form Button
Pada Praktikum ini, akan di tunjukkan bagaimana cara merubah warna background dan warna font hanya dengan mengklik tombol.

ketik kode berikut :

`<!DOCTYPE html>`
`<html lang="en">`
`<head>`
  `<meta charset="UTF-8">`
  `<meta http-equiv="X-UA-Compatible" content="IE=edge">`
  `<meta name="viewport" content="width=device-width, initial-scale=1.0">`
  `<title>objek document</title>`
`</head>`
`<body>`
  `<script lang="javascript">`
    function ubahWarnaLB(warna) {
      document.bgColor = warna;
    }
    function ubahWarnaLD(warna) {
      document.fgColor = warna;
    }
  `</script>`

  `<h1>Test</h1>`
  `<form>`
    `<input type="button" value="Latar Belakang Hijau" onclick="ubahWarnaLB('green')">`
    `<input type="button" value="Latar Belakang Putih" onclick="ubahWarnaLB('white')">`
    `<input type="button" value="teks kuning" onclick="ubahWarnaLD('yellow')">`
    `<input type="button" value="teks biru" onclick="ubahWarnaLD('blue')">`
  `</form>`
  `<script lang="javascript">`
    document.write("dimodifikasi terakhir pada " + document.lastModified);
  `</script>`
`</body>`
`</html>`

![Gambar23](screenshot/ss23.png)

Tampilan hasil pada browser.

![Gambar24](screenshot/ss24.png)


## 10. HTML DOM
Pilihan menggunakan checkBox dengan perhitungan otomatis. 

Ketiklah kode berikut.

`<!DOCTYPE html>`
`<html lang="en">`
`<head>`
  `<meta charset="UTF-8">`
  `<meta http-equiv="X-UA-Compatible" content="IE=edge">`
  `<meta name="viewport" content="width=device-width, initial-scale=1.0">`
  `<title>Daftar menu</title>`
  `<script>`
    function hitung(ele) {
      var total = document.getElementById('total').value;
          total = (total ? parseInt(total) : 0);
      var harga = 0;

      if (ele.checked) {
        harga = ele.value;
        total += parseInt(harga);
      } 
      else {
        harga = ele.value;
        if (total > 0)
            total -= parseInt(harga);
      }
      document.getElementById('total').value = total;
    }
  `</script>`
`</head>`
`<body>`
  `<h1>Daftar Menu Makanan</h1>`
  `<label><input type="checkbox" value="5000" id="menu1" onclick="hitung(this);" />Ayam Goreng Rp. 5000</label><br>`
  `<label><input type="checkbox" value="500" id="menu2" onclick="hitung(this);" />Tempe Goreng Rp. 500</label><br>`
  `<label><input type="checkbox" value="2500" id="menu3" onclick="hitung(this);" />Telur Dadar Rp. 2.500</label><br>`
  `<strong>Total Bayar: Rp. <input id="total" type="text"/></strong>`
`</body>`
`</html>`

![Gambar25](screenshot/ss25.png)

Tampilan hasil pada browser.

![Gambar26](screenshot/ss26.png)



## B. Tugas

Membuat script untuk melakukan validasi pada isian form.
Ketikan kode berikut.

`<!DOCTYPE html>`
`<html>`
`<head>`
    `<title>Membuat Form Validasi dengan Javascript</title>`
    `<link rel="stylesheet" type="text/css" href="Tugas.css">`
`</head>`
`<body>`
    `<!-- Judul -->`
    `<center><h2>Membuat Form Validasi</h2></center>`
`<div class="login">`
    `<form action="#" method="POST" onsubmit="validasi()">`
        `<div>`
            `<label>Nama Lengkap :</label>`
            `<input type="text" name="nama" id="nama"/>`
        `</div>`
        `<div>`
            `<label>Email :</label>`
            `<input type="email" name="email" id="email"/>`
        `</div>`
        `<div>`
            `<label>Alamat :</label>`
            `<textarea cols="40" rows="5" name="alamat" id="alamat"></textarea>`
        `</div>`
        `<div>`
            `<input type="submit" value="Daftar" class="tombol">`
        `</div>`

        `<footer>`
            `<hr>`
            `<p>2022 - Anggi Perdana - Form Validasi</p>`
            `<p>Universitas Pelita Bangsa</p>`
        `</footer>`
    `</form>`
`</div>`
`</body>`
`<script type="text/javascript">`
    function validasi() {
        var nama = document.getElementById("nama").value;
        var email = document.getElementById("email").value;
        var alamat = document.getElementById("alamat").value;
        if (nama != "" && email!="" && alamat !="") {
            return true;
        }else{
            alert('Anda harus mengisi data dengan lengkap !');
        }
    }
`</script>`
`</html>`

![Gambar27](screenshot/ss27.png)

Tambah dan buat juga file css berikut.

![Gambar28](screenshot/ss28.png)

Tampilan hasil form pada browser.

![Gambar29](screenshot/ss29.png)


Karena ini form validasi, maka apabila ada kesalahan atau kekurangan input, tampilannya akan seperti berikut ini. 

![Gambar30](screenshot/ss30.png)