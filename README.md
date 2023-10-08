# Pertanyaan Dan Tugas
## 2. Apa perbedaan pendeklarasian CSS elemen h1 {...} dengan #intro h1 {...}?

## "h1 {...}":
adalah selektor CSS umum yang mempengaruhi semua elemen "< h1 >". Dengan mendeklarasikan gaya CSS "h1 {...}", semua elemen < h1 > akan menerima gaya yang sama, tidak peduli di mana elemen-elemen tersebut berada dalam struktur dokumen HTML.

## intro h1 {...}:
adalah contoh dari selektor CSS yang lebih spesifik. Dalam hal ini, menggunakan "id" dengan nama "intro" untuk merujuk pada elemen yang memiliki id "intro". Kemudian, menentukan bahwa gaya CSS ini akan berlaku hanya untuk elemen < h1 > yang berada di dalam elemen dengan id "intro". Dengan kata lain, gaya CSS ini hanya akan mempengaruhi elemen < h1 > yang berada dalam konteks elemen dengan id "intro".

## 3. Apabila ada deklarasi CSS secara internal, lalu ditambahkan CSS eksternal dan inline CSS pada elemen yang sama. Deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya!

Ketika mendeklarasikan CSS secara internal (dalam elemen "< style >" di dalam halaman HTML), CSS eksternal (dalam file terpisah), dan inline CSS (langsung pada elemen HTML yang sama) yang semuanya berlaku pada elemen yang sama, urutan prioritas akan mempengaruhi bagaimana gaya ditampilkan oleh browser. Contohnya adalah sebagai berikut:

## Inline CSS:
Inline CSS memiliki prioritas tertinggi. Artinya, jika memberikan gaya CSS langsung pada elemen HTML dengan menggunakan atribut "style", maka gaya tersebut akan digunakan. Contoh
![Cuplikan layar 2023-10-08 122642](https://github.com/Diska404/Lab2Web/assets/115615910/9026e01b-aeb7-43dc-9085-4aa3e733077f)
Menjadi
![Cuplikan layar 2023-10-08 122719](https://github.com/Diska404/Lab2Web/assets/115615910/934b47c0-7951-4d68-8f21-f97723bac472)

## Internal CSS:
Deklarasi CSS yang ada dalam elemen < style > di dalam halaman HTML akan diterapkan setelah inline CSS. Jadi, jika memiliki deklarasi internal dan inline untuk elemen yang sama, deklarasi internal yang akan digunakan. Contoh
![Cuplikan layar 2023-10-08 132118](https://github.com/Diska404/Lab2Web/assets/115615910/9e399b01-9ca1-4c50-9183-87ec490a6d78)
Dalam contoh ini, warna teks akan menjadi biru karena deklarasi internal yang mengaturnya.

## Eksternal CSS:
Dalam file eksternal memiliki prioritas terendah. Ini diterapkan setelah deklarasi internal dan inline CSS. Jadi, jika memiliki deklarasi eksternal dan deklarasi internal atau inline untuk elemen yang sama, deklarasi eksternal yang akan digunakan. Contoh (misalkan file eksternal bernama "style.css"):
![Cuplikan layar 2023-10-08 132711](https://github.com/Diska404/Lab2Web/assets/115615910/eeb18a14-1076-45db-addf-bd426324be1e)


## 4. Pada sebuah elemen HTML terdapat ID dan Class, apabila masing-masing selector tersebut terdapat deklarasi CSS, maka deklarasi manakah yang akan ditampilkan pada browser? Berikan penjelasan dan contohnya! ( < p id="paragraf-1" class="text-paragraf"> )
Ketika sebuah elemen HTML memiliki ID dan Class yang terkait dengan deklarasi CSS, urutan prioritas akan mempengaruhi deklarasi CSS mana yang akan diterapkan pada elemen tersebut. Urutan prioritas CSS adalah sebagai berikut:

## ID Selector:
Deklarasi CSS yang menggunakan ID selector memiliki prioritas yang lebih tinggi daripada Class selector. Ini berarti jika ada deklarasi CSS yang menggunakan ID selector yang sesuai dengan elemen, deklarasi tersebut akan digunakan.

## Class Selector:
Jika tidak ada deklarasi CSS yang menggunakan ID selector yang sesuai dengan elemen, maka deklarasi CSS dengan Class selector akan diterapkan.

Contoh
![Cuplikan layar 2023-10-08 134015](https://github.com/Diska404/Lab2Web/assets/115615910/da2134cb-5f38-497a-b21f-45912e531049)

