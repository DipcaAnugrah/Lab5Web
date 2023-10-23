# Lab 5 Web

```
Nama    : Dipca Anugrah
NIM     : 312210666
Kelas   : TI.2.A.4
MATKUL  : Pemrograman Web 1
```

## **Daftar Isi**

**1. [Instruksi Praktikum](#instruksi-praktikum)**  
**2. [Langkah-langkah Praktikum](#langkah-langkah-praktikum)**  
**3. [Pertanyaan dan Tugas](#pertanyaan-dan-tugas)**

## **Instruksi Praktikum**

1. Persiapkan text editor misalnya VSCode.
2. Buat folder baru dengan nama Lab3Web
3. Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya.
4. Lakukan validasi dokumen html dengan mengakses http://validator.w3.org

## **Langkah-langkah Praktikum**

Persiapan membuat dokumen HTML dengan nama file **lab5_javascript.html** seperti berikut.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <title>Mengenal JavaScript</title>
  </head>
  <body>
    <h1>Pengenalan JavaScript</h1>
    <h3>Contoh document.write dan console.log</h3>
    <script>
      document.write("Hello World");
      console.log("Hello World");
    </script>
  </body>
</html>
```

![img](img_readme/langkah%201.png)

1.  **Javascrip Dasar**  
     Pemakaian Alert sebagai property window.
    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>alert box</title>
    </head>
    <body>
        <!-- Pemakaian Alert sebagai property window -->
        <script language = "javascript">
            window.alert("ini merupakan pesan untuk anda")
        </script>
    </body>
    </html>
    ```

    ![img](img_readme/langkah%202.png)

    <br>

    **Pemakaian method dalam objek**
    ```html
    <!DOCTYPE html>
        <html lang="en">
            <head>
                <meta charset="UTF-8">
                <meta name="viewport" content="width=device-width, initial-scale=1.0">
                <title>skrip javascript</title>
            </head>
            <body>
                percobaan memakai javascript:<br>
                <script language = "javascript">
                    document.write("selamat mencoba javascript<br>");
                    document.write("semoga sukses!");
                </script>
            </body>
        </html>
    ```

    ![img](img_readme/langkah%203.png)

    <br>

    **Pemakaian Prompt**

    ```html
    <!DOCTYPE html>
    <html lang="en">
        <head>
            <meta charset="UTF-8">
            <meta name="viewport" content="width=device-width, initial-scale=1.0">
            <title>pemasukan data</title>
        </head>
        <body>
            <script language = "javascript">
                var nama = prompt("siapa nama anda?", "masukkan nama anda");
                document.write("hai, " + nama);
            </script>
        </body>
    </html>
    ```
    [OUTPUT VIDEO](video/langkah%204.mp4)

    <br>

    **Pembuatan fungsi dan cara pemanggilannya**

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>contoh program JavaScript</title>
        <script language = "javascript">
            function pesan(){
                alert("memanggil javascript lewat body onload")
            }
        </script>
    </head>
    <body onload=pesan()>
        
    </body>
    </html>
    ```

    ![img](img_readme/langkah%205.png)

    <br>

2. **Dasar Pemrograman Di JavaScript**
    
    **Operasi dasar aritmatika**

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>contoh program JavaScript</title>
        <script language = "javascript">
            function test (val1, val2){
                document.write("<br>" + "perkalian : val1 * val2" + "<br>")
                document.write(val1*val2)
                document.write("<br>" + "pembagian : val1 / val2" + "<br>")
                document.write(val1/val2)
                document.write("<br>" + "penjumlahan : val1 + val2" + "<br>")
                document.write(val1+val2)
                document.write("<br>" + "pengurangan : val1 - val2" + "<br>")
                document.write(val1-val2)
                document.write("<br>" + "modulus : val1 % val2" + "<br>")
                document.write(val1%val2)
            }
        </script>
    </head>
    <body>
        <input type="button" name="button1" value="arithmetic" onclick=test(9,4)>
    </body>
    </html>
    ```
    [OUTPUT VIDEO](video/langkah%206.mp4)

    <br>

    **Seleksi kondisi (if..else)**

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>contoh if-else</title>
    </head>
    <body>
        <script language="javascript">
            var nilai = prompt("nilai (0-100): ", 0);
            var hasil = "";
            if (nilai >= 60)
            hasil = "lulus";
            else
            hasil = "tidak lulus";
            document.write("hasil: " + hasil);
        </script>
    </body>
    </html>
    ```
    [OUTPUT VIDEO](video/langkah%207.mp4)

    <br>

    **Penggunaan operator switch untuk seleksi kondisi**

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>contoh program javascript</title>

        <script language = "javascript">
            function test (){
                val1 = window.prompt("input nilai (1-5)")
                switch (val1){
                    case "1" : 
                        document.write("bilangan satu")
                        break
                    case "2" : 
                        document.write("bilangan dua")
                        break
                    case "3" : 
                        document.write("bilangan tiga")
                        break
                    case "4" : 
                        document.write("bilangan empat")
                        break
                    case "5" : 
                        document.write("bilangan lima")
                        break
                    default : 
                        document.write("bilangan lainnya")
                }
            }
        </script>
    </head>
    <body>
        <input type="button" name="button1" value="switch" onclick=test()>
    </body>
    </html>
    ```
    [OUTPUT VIDEO](video/langkah%208.mp4)

    <br>

3. **Pembuatan Form**

    **Form Input**

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Form input</title>

        <script language="javascript">
            function test () {
                var val1 = document.kirim.T1.value
                if (val1%2==0)
                    document.kirim.T2.value = "bilangan genap"
                else   
                    document.kirim.T2.value = "bilangan ganjil"
            }
        </script>
    </head>
    <body>
        <form method="POST" name="kirim">
            <p>BIL <input type="text" name="T1" size="20">
            MERUPAKAN BIL <input type="text" name="T2" size="20"></p>
            <p><input type="button" name="B1" value="TEBAK" onclick=test()></p>
        </form>
    </body>
    </html>
    ```
    [OUTPUT VIDEO](video/langkah%209.mp4)

    <br>

    **Form Button**

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Form button - objek document</title>
    </head>
    <body>
        <script language = "javascript">
            function ubahWarnaLB(warna) {
                document.bgColor = warna;
            }
            function ubahWarnaLD(warna) {
                document.fgColor = warna;
            }
        </script>

        <h1>tes</h1>
        <form>
            <input type="button" value="Latar Belakang Hijau" onclick="ubahWarnaLB('GREEN')">
            <input type="button" value="Latar Belakang Putih" onclick="ubahWarnaLB('WHITE')">
            <input type="button" value="Teks Kuning" onclick="ubahWarnaLD('YELLOW')">
            <input type="button" value="Teks Biru" onclick="ubahWarnaLD('BLUE')">
        </form>

        <script language = "javascript">
            document.write("Dimodivikasi terakhir pada " + document.lastModified);
        </script>
    </body>
    </html>
    ```
    [OUTPUT VIDEO](video/langkah%2010.mp4)

    <br>

4. **HTML DOM**

    **Pilihan menggunakan checkbox dengan perhitungan otomatis**

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Daftar Menu</title>

        <script>
            function hitung(ele) {
                var total = document.getElementById('total').value;
                total = total ? parseInt(total) : 0;
                var harga = 0;

                if (ele.checked) {
                    harga = ele.getAttribute('value'); // Mengambil nilai dari atribut 'value'
                    total += parseInt(harga);
                } else {
                    harga = ele.getAttribute('value'); // Mengambil nilai dari atribut 'value'
                    if (total > 0) {
                        total -= parseInt(harga);
                    }
                }

                document.getElementById('total').value = total;
            }
        </script>
    </head>
    <body>
        <h1>Daftar Menu</h1>

        <label><input type="checkbox" value="5000" id="menu1" onclick="hitung(this);"> Ayam Goreng Rp. 5.000</label>
        <br>
        <label><input type="checkbox" value="500" id="menu2" onclick="hitung(this);"> Tempe Goreng Rp. 500</label>
        <br>
        <label><input type="checkbox" value="2500" id="menu3" onclick="hitung(this);"> Telur Dadar Rp. 2.500</label>
        <hr>

        <strong> Total Bayar: Rp. <input type="text" id="total"></strong>

    </body>
    </html>

    ```
    [OUTPUT VIDEO](video/langkah%2011.mp4)


## Pertanyaan dan Tugas
1. **Buat script untuk melakukan validasi pada isian form.**

    ```html
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <title>Formulir Validasi</title>

        <!-- my styles css -->
        <link rel="stylesheet" href="../css/styles.css">
        <script>
            function validateForm() {
                // Dapatkan referensi ke elemen-elemen formulir
                var nama = document.forms["myForm"]["nama"].value;
                var email = document.forms["myForm"]["email"].value;

                // Lakukan validasi
                if (nama == "") {
                    alert("Nama wajib diisi");
                    return false;
                }

                if (email == "") {
                    alert("Email wajib diisi");
                    return false;
                }

                // Validasi apakah email sesuai dengan format yang benar
                var emailPattern = /^[a-zA-Z0-9._-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,4}$/;

                if (!emailPattern.test(email)) {
                    alert("Email tidak valid. Harap masukkan alamat email yang benar.");
                    return false;
                }
            }
        </script>
    </head>
    <body>
        <h1>Formulir Validasi</h1>
        <div class="container">
            <form name="myForm" onsubmit="return validateForm()" method="post">
                <div class="input-group">
                    <label for="nama"><img src="../img/user (3).svg" class="label-img"></label>
                    <input type="text" id="nama" name="nama" placeholder="Nama" class="input">
                </div>
                
                <div class="input-group">
                    <label for="email"><img src="../img/mail.svg" class="label-img"></label>
                    <input type="text" id="email" name="email" placeholder="Email" class="input">
                </div>
                
        
                <input type="submit" value="Submit" class="btn">
            </form>
        </div>
        
    </body>
    </html>

    ```
    [OUTPUT VIDEO](video/langkah%2012.mp4)


**[---BACK-->](#lab-5-web)**