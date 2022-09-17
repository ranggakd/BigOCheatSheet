# BigOCheatSheet

* [Pengenalan](#pengenalan)
* [Kompleksitas Komputasi Asimtotik](#kompleksitas-komputasi-asimtotik)
* [Asimtot](#asimtot)
* [Analisis Asimtot](#analisis-asimtot)
* [Big O](#big-o)
* [Big Omega](#big-ω)
* [Big Theta](#big-θ)
* [Perbedaan Ketiganya](#perbedaan-ketiganya)
* [Konteks Kasus Terburuk, Terbaik, Rata-rata](#konteks-kasus-terburuk-terbaik-rata-rata)
* [Referensi](#referensi)

## Pengenalan

Sebelum kita menuju ke situs, kita perlu tahu dahulu apa itu __Kompleksitas Komputasi Asimtotik__. Jika dirimu sudah familiar dengan istilah ini, lewati dan langsung menuju ke [Big-O Cheat Sheet Website](https://www.bigocheatsheet.com/).

![ilustrasi_big_notation](big.png)

**[🔝 kembali ke atas](#bigocheatsheet)**

## Kompleksitas Komputasi Asimtotik

> Dalam teori kompleksitas komputasi, __kompleksitas komputasi asimtotik__ merupakan penggunaan __analisis asimtotik__ untuk _estimasi kompleksitas komputasi algoritme dan masalah komputasi_, yang umumnya dikaitkan dengan penggunaan notasi _big O_. - [Wikipedia](https://en.wikipedia.org/wiki/Asymptotic_computational_complexity)

Untuk memahami istilah-istilah tersebut, kita perlu tahu dahulu apa itu __Asimtot__ sebelum kita menyelam dalam __Analisis Asimtotik__.

**[🔝 kembali ke atas](#bigocheatsheet)**

## Asimtot

> Dalam geometri analitis, __asimtot__ dari sebuah kurva adalah sebuah garis yang sedemikian rupa sehingga jarak antara kurva dan garis tersebut mendekati nol seiring x atau y (salah satu atau keduanya) mendekati takhingga. - [Wikipedia](https://id.wikipedia.org/wiki/Asimtot)

Berikut contoh visual dari [jarednielsen](https://jarednielsen.com/static/32c1589243f13448fac04d22cb735af9/40601/desmos-asymptote-01.png)

    y = 1/x
![function of 1/x](https://jarednielsen.com/static/32c1589243f13448fac04d22cb735af9/40601/desmos-asymptote-01.png)

> __Tak peduli seberapa besar atau kecil nilai x, kurva tidak akan pernah menyentuh sumbu x atau y__. Bahkan jika nilainya takhingga. 🐢🏃‍♀️.Terutama jika nilainya nol. Mengapa? Secara matematis tidak mungkin untuk membagi dengan nol. Pada grafik diatas, __sumbu x dan y__ merupakan __asimtot dari persamaan__ `y = 1 / x`. Namun garis apapun bisa menjadi asimtot. Tidak terbatas pada garis horizontal dan vertikal. - [jarednielsen](https://jarednielsen.com/big-o-omega-theta/)

Sekarang kita dapat ide tentang __asimtot__, ayo lanjut mempelajari mengenai __Analisis Asimtotik__.

**[🔝 kembali ke atas](#bigocheatsheet)**

## Analisis Asimtot

> Dalam analisis matematis, __analisis asimtotik__, juga disebut sebagai __asimtotik_ merupakan _metode untuk menggambarkan perilaku limit_. - [Wikipedia](https://en.wikipedia.org/wiki/Asymptotic_analysis)

Sebagai contoh kita dapat dari [jarednielsen](https://jarednielsen.com/big-o-omega-theta/). Diberikan fungsi `f(x) = x^2 + 2x`, dimana `x` nilainya meningkat (mendekati takhingga) dan `2x` menjadi tak signifikan dibandingkan dengan `x^2`. Sederhananya, kita dapat katakan `f(x)` ekuivalen secara asimtotik dengan `x^2`.

Mengapa kita perlu __analisis asimtotik__ ini dirimu mungkin bertanya?

Karena kita perlu mengestimasi kompleksitas komputasional dari algoritme dan masalah komputasional. Agar semua orang sepakat pada hal yang sama, kita menggunakan notasi-notasi ini: __big O, big Ω and big θ__ untuk menggambarkan tipe estimasi yang berbeda.

**[🔝 kembali ke atas](#bigocheatsheet)**

## Big O

> __Big O__ menggambarkan __batas atas__ suatu algoritme. Inilah mengapa, kita sebagai pengembang dan praktisi terutama peduli dengan Big O. Kita ingin tahu _seberapa buruk kinerja suatu algoritme_. - [jarednielsen](https://jarednielsen.com/big-o-omega-theta/)

> Ini didefinisikan sebagai batas atas dan __batas atas pada suatu algoritme__ merupakan jumlah waktu paling banyak yang dibutuhkan (kinerja kasus terburuk). Notasi __Big O__ digunakan untuk menggambarkan __batas atas asimtotik__. - [GeeksForGeeks](https://www.geeksforgeeks.org/difference-between-big-oh-big-omega-and-big-theta/)

![bigO_gfg](https://media.geeksforgeeks.org/wp-content/cdn-uploads/20200807150308/3363.png)

**[🔝 kembali ke atas](#bigocheatsheet)**

## Big Ω

> __Big Omega__ menggambarkan __batas bawah__ suatu algoritme. Kalo saja hidup selalu memberi kita array yang diurutkan. 🌼. Kita juga dapat menganggap ini sebagai _skenario kasus terbaik_ kita. - [jarednielsen](https://jarednielsen.com/big-o-omega-theta/)

> Ini didefinisikan sebagai batas bawah dan __batas bawah pada suatu algoritme__ merupakan jumlah paling sedikit yang dibutuhkan (cara yang paling efisien, dengan kata lain kasus terbaik). Seperti notasi O menyediakan batas atas asimtotik, __notasi Ω__ menyediakan __batas bawah asimtotik__. - [GeeksForGeeks](https://www.geeksforgeeks.org/difference-between-big-oh-big-omega-and-big-theta/)

![bigomega_gfg](https://media.geeksforgeeks.org/wp-content/cdn-uploads/20200807150659/3611.png)

**[🔝 kembali ke atas](#bigocheatsheet)**

## Big θ

> __Big Theta__ menggambarkan __batasan ketat__ suatu algoritme, batasannya dari atas dan bawah. Big Theta sering digunakan untuk menggambarkan _kasus rata-rata atau yang diharapkan_ untuk suatu algoritme. Ini tidak sepenuhnya benar, tetapi ini adalah singkatan yang berguna. - [jarednielsen](https://jarednielsen.com/big-o-omega-theta/)

> Ini didefinisikan sebagai batas terketat dan __batas terketat__ merupakan yang terbaik dari semua waktu kasus terburuk yang dapat diambil oleh algoritme. - [GeeksForGeeks](https://www.geeksforgeeks.org/difference-between-big-oh-big-omega-and-big-theta/)

![bigtheta_gfg](https://media.geeksforgeeks.org/wp-content/cdn-uploads/20200807150743/36955.png)

**[🔝 kembali ke atas](#bigocheatsheet)**

## Perbedaan Ketiganya

| | Big O | Big Ω / Omega | Big θ / Theta |
| :--- | :---: | :---: | :---: |
| Operator bersyarat | `<=` | `>=` | `==`
| Tingkat pertumbuhan suatu algoritme / struktur data | kurang dari | lebih dari | sama dengan |
| Batas | atas | bawah | atas dan bawah |
| Notasi | `O(n)` | `Ω(n)` | `θ(n)` |

**[🔝 kembali ke atas](#bigocheatsheet)**

## Konteks Kasus Terburuk, Terbaik, Rata-rata

Apa hubungan antara
> __kasus terbaik__ / __kasus terburuk__ / __kasus diharapkan__

dengan

> __Big O__ / __Big Omega (Ω)__ / __Big Theta (θ)__?

__Tidak ada__. 

> Ekuivalensi sering dibuat antara __Big O dan kasus terburuk__, __Big Omega dan kasus terbaik__, dan __Big Theta dan kasus rata-rata__ untuk __setiap notasi__. - [jarednielsen](https://jarednielsen.com/big-o-omega-theta/)

> Misalnya, setiap pernyataan mengenai __kasus terburuk__ berikut ini semuanya benar:
>> Tingkat pertumbuhan kasus terburuk Insertion Sort __paling tinggi__ `O(n^2)`  
>> Tingkat pertumbuhan kasus terburuk Insertion Sort __paling rendah__ `Ω(n)`  
>> Tingkat pertumbuhan kasus terburuk Insertion Sort __tepat__ `Θ(n^2)`

**[🔝 kembali ke atas](#bigocheatsheet)**

## Referensi

[Big-O Cheat Sheet Website](https://www.bigocheatsheet.com/) ◽ diakses terakhir 17 September 2022

[Asymptotic computational complexity](https://en.wikipedia.org/wiki/Asymptotic_computational_complexity) ◽ diakses terakhir 17 September 2022

[Asimtot](https://id.wikipedia.org/wiki/Asimtot) ◽ diakses terakhir 17 September 2022

[Asymptotic analysis](https://en.wikipedia.org/wiki/Asymptotic_analysis) ◽ diakses terakhir 17 September 2022

[What’s the Difference Between Big O, Big Omega, and Big Theta?](https://jarednielsen.com/big-o-omega-theta/) ◽ diakses terakhir 17 September 2022

[Difference between Big Oh, Big Omega and Big Theta](https://www.geeksforgeeks.org/difference-between-big-oh-big-omega-and-big-theta/) ◽ diakses terakhir 17 September 2022

**[🔝 kembali ke atas](#bigocheatsheet)**