# lab3web
# LAPORAN PRAKTIKUM 3

## CSS DASAR

### Identitas Mahasiswa

* **Nama:** sairin bin rubad
* **NIM:** 312510134
* **Program Studi:** Teknik Informatika
* **Mata Kuliah:** Pemrograman Web
* **Praktikum:** Praktikum 3 — CSS Dasar

---

## Pengertian CSS

Cascading Style Sheet (CSS) merupakan aturan yang digunakan untuk mengatur berbagai komponen dalam sebuah halaman web agar tampilannya lebih terstruktur dan seragam. CSS bukan merupakan bahasa pemrograman, tetapi digunakan untuk mengatur tampilan dari dokumen HTML.

Dengan CSS, tampilan pada beberapa halaman web dapat diubah secara lebih mudah. CSS juga memiliki berbagai atribut yang dapat digunakan untuk mengatur warna, ukuran teks, posisi, jarak, background, dan tampilan elemen HTML lainnya.

---

# Langkah-Langkah Praktikum

## 1. Membuat Dokumen HTML

### Tujuan

Membuat struktur dasar dokumen HTML yang akan digunakan sebagai dasar untuk menerapkan CSS.

### CODING

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CSS Dasar</title>
</head>

<body>

    <header>
        <h1>CSS Internal dan <i>Inline CSS</i></h1>
    </header>

    <nav>
        <a href="lab2_css_dasar.html">CSS Dasar</a>
        <a href="lab2_css_eksternal.html">CSS Eksternal</a>
        <a href="lab1_tag_dasar.html">HTML Dasar</a>
    </nav>

    <div id="intro">
        <h1>Hello World</h1>

        <p>
            Kami sedang belajar HTML dan CSS dasar, pada mata kuliah
            <b>Pemrograman Web</b> di <i>Universitas Pelita Bangsa</i>.
            Pelajaran pertama yang kami dapat adalah membuat tampilan
            web sederhana dalam rangka mengenal tag-tag dasar HTML dan CSS.
        </p>

        <a class="button btn-primary" href="#intro">
            Informasi selengkapnya.
        </a>
    </div>

</body>
</html>
```

### Screenshot Codingan


<img width="1521" height="1262" alt="codingan 1" src="https://github.com/user-attachments/assets/488ab6ad-5207-41f9-96a3-7d88c39834dc" />


### Hasil Browser


<img width="1876" height="446" alt="hasil-browser 1" src="https://github.com/user-attachments/assets/277c9806-5d22-437d-98ef-3a44b8099578" />


### Keterangan

Pada langkah pertama dibuat struktur dasar HTML yang terdiri dari `header`, `nav`, dan bagian `div` dengan ID `intro`. Struktur ini nantinya digunakan sebagai dasar untuk menerapkan CSS.

---

## 2. Mendeklarasikan CSS Internal

### Tujuan

Menambahkan CSS secara internal pada bagian `<head>` dokumen HTML.

### CODING

```html
<head>
    <title>CSS Dasar</title>

    <style>
        body {
            font-family: 'Open Sans', sans-serif;
        }

        header {
            min-height: 80px;
            border-bottom: 1px solid #77CCEF;
        }

        h1 {
            font-size: 24px;
            color: #0F189F;
            text-align: center;
            padding: 20px 10px;
        }

        h1 i {
            color: #6d6a6b;
        }
    </style>
</head>
```

### Screenshot Codingan


<img width="745" height="789" alt="codingan 2" src="https://github.com/user-attachments/assets/59004e5f-bbc4-4d25-9954-a06eb490ff70" />


### Hasil Browser


<img width="1858" height="507" alt="hasil-browser 2" src="https://github.com/user-attachments/assets/f9217947-febd-4f13-a05c-b9c68b4f3bac" />


### Keterangan

CSS Internal dituliskan di dalam tag `<style>` yang berada pada bagian `<head>`. Pada langkah ini CSS digunakan untuk mengatur jenis font, tinggi header, garis bawah header, ukuran heading, warna, posisi teks, dan warna teks italic.

---

## 3. Menambahkan Inline CSS

### Tujuan

Menerapkan CSS secara langsung pada elemen HTML menggunakan atribut `style`.

### CODING

```html
<p style="text-align: center; color: #ccd8e4;">
</p>
```

### Screenshot Codingan


<img width="1486" height="211" alt="codingan 3" src="https://github.com/user-attachments/assets/4c58c29e-2b62-4bce-967c-487827fb52cc" />


### Hasil Browser


<img width="1877" height="532" alt="hasil-browser 3" src="https://github.com/user-attachments/assets/7f18db9b-aab5-4ccb-abbc-663905acd492" />


### Keterangan

Inline CSS ditambahkan langsung pada tag HTML menggunakan atribut `style`. CSS secara inline hanya memengaruhi elemen tempat kode tersebut dituliskan.

---

## 4. Membuat CSS Eksternal

### Tujuan

Membuat file CSS terpisah sehingga aturan CSS tidak berada langsung di dalam dokumen HTML.

### Nama File

```text
style_eksternal.css
```

### CODING

```css
body {
    color: blue;
}

p {
    font-family: "sans-serif";
}

h1 {
    text-align: center;
    color: red;
}

p {
    text-align: justify;
    color: green;
    font-size: 12pt;
}
```

Kemudian hubungkan file CSS dengan HTML menggunakan:

```html
<head>
    <link rel="stylesheet"
          href="style_eksternal.css"
          type="text/css">
</head>
```

### Screenshot Codingan


<img width="691" height="441" alt="codingan 4" src="https://github.com/user-attachments/assets/44f6fca5-29cf-4428-9f87-d3020a7e87df" />

<img width="714" height="194" alt="codingan 4 2" src="https://github.com/user-attachments/assets/9fa48fc6-3307-41d1-9ce1-c367b6c7196c" />



### Hasil Browser


<img width="1907" height="570" alt="hasil-browser 4" src="https://github.com/user-attachments/assets/25f04ea7-2244-42a6-aa72-5d8523af5d87" />


### Keterangan

CSS Eksternal dibuat dalam file terpisah dengan ekstensi `.css`. File tersebut kemudian dihubungkan dengan dokumen HTML menggunakan tag `<link>` pada bagian `<head>`.

---

## 5. Menambahkan CSS Selector

### Tujuan

Menerapkan CSS Selector menggunakan ID Selector dan Class Selector.

### CODING

#### ID Selector

```css
#intro {
    background: #418fb1;
    border: 1px solid #099249;
    min-height: 100px;
    padding: 10px;
}

#intro h1 {
    text-align: left;
    border: 0;
    color: #fff;
}
```

#### Class Selector

```css
.button {
    padding: 15px 20px;
    background: #bebcbd;
    color: #fff;
    display: inline-block;
    margin: 10px;
    text-decoration: none;
}

.btn-primary {
    background: #E42A42;
}
```

### Screenshot Codingan


<img width="640" height="526" alt="codingan 5" src="https://github.com/user-attachments/assets/3994fb6a-d4e8-4767-87f4-dab304f3ff10" />


### Hasil Browser


<img width="1902" height="659" alt="hasil-browser 5" src="https://github.com/user-attachments/assets/bba77e52-840d-47ed-a9fd-98e61f0e423d" />


### Keterangan

CSS Selector digunakan untuk menentukan elemen HTML yang akan diberikan aturan CSS.

ID Selector menggunakan tanda `#` sebelum nama ID, sedangkan Class Selector menggunakan tanda titik `.` sebelum nama class.

Pada HTML digunakan:

```html
<div id="intro">
```

dan:

```html
<a class="button btn-primary" href="#intro">
    Informasi selengkapnya.
</a>
```

---

# Pertanyaan dan Tugas

# Pertanyaan dan Tugas

## 1. Eksperimen Properti dan Nilai CSS

Eksperimen dilakukan dengan mengubah atau menambahkan properti dan nilai CSS untuk melihat perubahan tampilan pada halaman web. Beberapa properti yang dapat dicoba antara lain `background-color` untuk mengubah warna latar belakang, `font-size` untuk mengatur ukuran tulisan, `color` untuk mengubah warna teks, `padding` untuk mengatur jarak bagian dalam elemen, dan `border` untuk memberikan garis pada elemen. Dengan melakukan eksperimen, dapat diketahui fungsi dari setiap properti dan pengaruhnya terhadap tampilan halaman.

---

## 2. Perbedaan `h1 { ... }` dengan `#intro h1 { ... }`

Selector `h1 { ... }` digunakan untuk memberikan CSS kepada semua elemen `<h1>` yang terdapat pada halaman. Sedangkan `#intro h1 { ... }` hanya memberikan CSS kepada elemen `<h1>` yang berada di dalam elemen yang memiliki `id="intro"`. Selector `#intro h1` lebih spesifik karena menentukan lokasi elemen yang akan diberi style.

---

## 3. CSS Internal, Eksternal, dan Inline

Jika CSS Internal, CSS Eksternal, dan Inline CSS diterapkan pada elemen yang sama dan memiliki properti yang sama, maka aturan CSS dengan prioritas yang lebih tinggi akan diterapkan. Inline CSS memiliki prioritas lebih tinggi dibandingkan CSS Internal dan CSS Eksternal.

Contohnya, jika CSS Internal dan External memberikan warna biru, sedangkan Inline CSS memberikan warna merah, maka teks akan tampil berwarna merah karena Inline CSS memiliki prioritas yang lebih tinggi.

---

## 4. ID dan Class pada Elemen yang Sama

Jika satu elemen HTML memiliki `id` dan `class`, kemudian keduanya memiliki aturan CSS untuk properti yang sama, maka ID Selector memiliki tingkat kekhususan yang lebih tinggi dibandingkan Class Selector.

Contohnya, jika `#paragraf-1` memberikan warna merah dan `.text-paragraf` memberikan warna biru pada elemen yang sama, maka teks akan tampil berwarna merah karena ID Selector memiliki prioritas yang lebih tinggi daripada Class Selector.


---

# Kesimpulan

CSS digunakan untuk mengatur tampilan dan memberikan desain pada halaman HTML. Pada praktikum ini dipelajari struktur CSS yang terdiri dari selector, property, dan value serta tiga cara penerapan CSS yaitu Internal CSS, External CSS, dan Inline CSS.

Selain itu, dipelajari juga penggunaan Element Selector, ID Selector, dan Class Selector. Dengan menggunakan CSS, tampilan halaman HTML dapat diatur menjadi lebih terstruktur dan menarik.

---

# Dokumentasi

Struktur folder praktikum:

```text
Lab3Web/
│
├── lab2_css_dasar.html
├── style_eksternal.css
├── README.md
│
└── images/
    ├── codingan 1.png
    ├── hasil-browser 1.png
    ├── codingan 2.png
    ├── hasil-browser 2.png
    ├── codingan 3.png
    ├── hasil-browser 3.png
    ├── codingan 4.png
    ├── hasil-browser 4.png
    ├── codingan 5.png
    ├── hasil-browser 5.png
    
```

Screenshot digunakan pada setiap perubahan praktikum sesuai ketentuan laporan.
