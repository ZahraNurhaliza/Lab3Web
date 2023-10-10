# Lab3Web

## Langkah-langkah Praktikum
1. Persiapan membuat dokumen HTML dengan nama file lab3_list.html seperti berikut.
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>
        <h1>Membuat List</h1>
    </header>
</body>
</html>
```
2. Membuat Ordered List
Kemudian tambahkan kode untuk membuat Ordered List seperti berikut.
```html
 <section id="order-list">
        <h2>Ordered List</h2>
        <ol>
        <li>Pemrograman Web</li>
        <li>Sistem Informasi</li>
        <li>Basis Data 2</li>
        </ol>
    </section>
```
![image](https://github.com/ZahraNurhaliza/Lab3Web/blob/main/screenshot/ss.1.png)


3. Membuat Unorderd List
Kemudian tambakan kode untuk membuat Unordered List, setelah deklarasi ordered list pada
section unordered-list, seperti berikut.
```html
 <section id="unorder-list">
        <h2>Unordered List</h2>
        <ul type="square">
        <li>Jaringan Komputer</li>
        <li>Struktur Data</li>
        <li>Algoritma &amp; Pemrograman</li>
    </ul>
    </section>
```
![image](https://github.com/ZahraNurhaliza/Lab3Web/blob/main/screenshot/ss.2.png)


4. Membuat Description List
Kemudian tambahkan kode untuk membuat description list setelah deklarasi unorderd-list.4.
```html
<section id="unorder-list">
        <h2>Description List</h2>
        <dl>
            <dt>Fakultas Teknik</dt>
            <dd>Teknik Industri</dd>
            <dd>Teknik Informatika</dd>
            <dd>Teknik Lingkungan</dd>
            <dt>Fakultas Ekonomi dan Bisnis</dt>
            <dd>Akuntansi</dd>
            <dd>Manajemen</dd>
            <dd>Bisnis Digital</dd>
        </dl>
    </section>
```
![image](https://github.com/ZahraNurhaliza/Lab3Web/blob/main/screenshot/ss.3.png)


5. Membuat Tabel
Buat file baru dengan nama lab3_tabel.html seperti berikut.
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>
        <h1>Membuat Table</h1>
    </header>
    <table border="1" cellpadding="4" cellspacing="0">
        <thead>
            <tr>
                <th>No.</th>
                <th>Fakultas</th>
                <th>Program Studi</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>1.</td>
                <td>Teknik</td>
                <td>Teknik Informatika</td>
            </tr>
            <tr>
                <td>2.</td>
                <td>Teknik</td>
                <td>Teknik Industri</td>
            </tr>
            <tr>
                <td>3.</td>
                <td>Teknik</td>
                <td>Teknik Lingkungan</td>
            </tr>
        </tbody>
    </table>
</body>
</html>
```
![image](https://github.com/ZahraNurhaliza/Lab3Web/blob/main/screenshot/ss.4.png)


6. Menggabungkan Sel Data
Untuk menggabungkan sel data, gunakan atribut rowspan dan colspan. Atribut rowspan untuk
menggabungkan baris (secara vertikal) dan colspan untuk menggabungkan kolom (secara
horizontal).
```html
<table border="1" cellpadding="6" cellspacing="0">
        <thead>
            <tr>
                <th>No.</th>
                <th>Fakultas</th>
                <th>Program Studi</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>1.</td>
                <td rowspan="3">Teknik</td>
                <td>Teknik Informatika</td>
            </tr>
            <tr>
                <td>2.</td>
                <td>Teknik Industri</td>
            </tr>
            <tr>
                <td>3.</td>
                <td>Teknik Lingkungan</td>
            </tr>
        </tbody>
    </table>
```
![image](https://github.com/ZahraNurhaliza/Lab3Web/blob/main/screenshot/ss.5.png)


7. Membuat Form
Buat file baru dengan nama lab3_form.html seperti berikut.
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML Lanjutan</title>
</head>
<body>
    <header>
        <h1>Membuat Form</h1>
    </header>
    <form action="proses.php" method="post">
        <fieldset>
            <legend>Data Pelanggan</legend>
            <p>
                <label for="nama">Nama</label>
                <input type="text" id="nama" name="nama">
            </p>
            <p>
                <label for="alamat">Alamat</label>
                <textarea id="alamat" name="alamat" cols="20" rows="3"></textarea>
            </p>
            <p>
                <label>Jenis Kelamin</label>
                <input id="jk_l" type="radio" name="kelamin" value="L" /><label
    for="jk_l">Laki-laki</label>
                <input id="jk_p" type="radio" name="kelamin" value="P" /><label
    for="jk_p">Perempuan</label>
            </p>
            <p><input type="submit" value="Login"></p>
        </fieldset>
</form>
</body>
</html>
```
![image](https://github.com/ZahraNurhaliza/Lab3Web/blob/main/screenshot/ss.6.png)


8. Menabahkan Style pada Form
Tambahkan syntax ini di bagian head (lab3_form.html)
```html
<link rel="stylesheet" href="style.css" type="text/css">
```
Agar tampilan form lebih menarik, bisa ditambahkan CSS seperti berikut.
```css
form p > label {
    display: inline-block;
    width: 100px;
}
form input[type="text"], form textarea {
    border: 1px solid #197a43;
}
form input[type="submit"] {
    border: 1px solid #197a43;
    background-color: #197a43;
    color: #ffffff;
    font-weight: bold;
    padding: 5px 15px;
}
```
![image](https://github.com/ZahraNurhaliza/Lab3Web/blob/main/screenshot/ss.7.png)



## Pertanyaan dan Tugas
1. Buatlah form yang menampilkan dropdown menu dan listbox dengan multiple selection.
```html
<p>
                <label for="Kpop Idol">Pilih Kpop Idol:</label>
                <select id="Kpop Idol" name="Kpop Idol">
                    <option value="EXO">EXO</option>
                    <option value="NCT">NCT</option>
                    <option value="Treasure">Treasure</option>
                    <option value="DAY6">DAY6</option>
                    <option value="Seventeen">Seventeen</option>
                </select>
            </p>
            <p>
                <label for="BIAS">Pilih BIAS:</label>
                <select id="BIAS" name="BIAS" multiple>
                    <option value="Chanyeol">Chanyeol</option>
                    <option value="Jamein">Jamein</option>
                    <option value="Yuta">Yuta</option>
                    <option value="Jisung">Jisung</option>
                    <option value="Junghwa">Junghwa</option>
                    <option value="Wonpil">Wonpil</option>
                    <option value="Wonwoo">Wonwoo</option>
                </select>
            </p>
```
![image](https://github.com/ZahraNurhaliza/Lab3Web/blob/main/screenshot/ss.8.png)

## SELESAI