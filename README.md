# Lab9web

Nama &nbsp; &nbsp;: Bayu Maulana Ayassy<br>
NIM&nbsp; &nbsp; &nbsp; : 312210166<br>
Kelas&ensp; &nbsp; : TI.22.A.1<br>

## Instruksi Praktikum
1. Persiapkan text editor misalnya VSCode

2. Buat folder baru dengan nama `lab9_php_modular` pada docroot webserver (htdocs)

3. Ikuti langkah-langkah praktikum yang akan dijelaskan berikutnya

## Langkah-langkah Praktikum
- Jalankan Apache dan MySQL server dari menu XAMPP Control
- Kemudian buat folder baru dengan nama lab9_php_modular pada docroot webserver (c:\xampp\htdocs). Kemudian buka melalui browser dengan mengakses URL: http://localhost/lab9_php_modular/.

![1](https://github.com/syifaaurellia/Lab9web/assets/115867244/ab5f4256-e26d-47be-974b-67e51867e1aa)

1. Buat file dengan nama `header.php`
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Contoh Modularisasi</title>
    <link href="style.css" rel="stylesheet" type="text/stylesheet" media="screen" />
</head>
<body>
    <div class="container">
        <header>
            <h1>Modularisasi Menggunakan Require</h1>
        </header>
        <nav>
            <a href="home.php">Home</a>
            <a href="about.php">Tentang</a>
            <a href="kontak.php">Kontak</a>
        </nav>
```

2. Buat file dengan nama `footer.php`
```
        <footer>
            <p>&copy; 2021, Informatika, Universitas Pelita Bangsa</p>
        </footer>
    </div>
</body>
</html>
```

3. Buat file dengan nama `home.php`
```
<?php require('header.php'); ?>

<div class="content">
    <h2>Ini Halaman Home</h2>
    <p>Ini adalah bagian content dari halaman.</p>
</div>

<?php require('footer.php'); ?>
```

4. Buat file dengan nama `about.php`
```
<?php require('header.php'); ?>

<div class="content">
    <h2>Ini Halaman About</h2>
    <p>Ini adalah bagian content dari halaman.</p>
</div>

<?php require('footer.php'); ?>
```

- Output halaman `Home` :
![2](https://github.com/syifaaurellia/Lab9web/assets/115867244/c1058bc0-3584-4a84-865d-046af8369cfc)


- Output halaman `About` :
![3](https://github.com/syifaaurellia/Lab9web/assets/115867244/51313ca1-49ee-4552-914e-6e2abc1ce828)

