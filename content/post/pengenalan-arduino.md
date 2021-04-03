---
title : "Pengenalan Arduino"
date : 2021-04-02T08:11:12Z
author : "Saiful Miqdar"
tags : [
	"arduino",
]
thumbnail : "images/arduino/arduino_uno.jpg"
description : "Tutorial belajar dasar arduino bagi pemula"
draft : false
---


# Apa itu Arduino?

Arduino adalah micro kontroller open source yang dirancang untuk memudahkan pembuatan proyek - proyek elektronika dalam berbagai bidang.

# Apa itu open source ?

Open source adalah perangkat lunak dimana kode program nya terbuka dan disediakan oleh pengembangnya secara umum agar dapat dipelajari, diubah atau dikembangkan lebih lanjut dan disebar luaskan.

# Apa kelebihan Arduino?

Kelebihan Arduino yaitu memiliki bootloader sendiri, murah, mudah dipelajari, punya banyak library gratis, menggunakan port USB, bersifat open source, dan masih banyak lagi.

# Apa Fungsi Arduino ?

Seperti kita ketahui, sebuah mikrokontroler dapat membuat program untuk mengendalikan berbagai komponen elektronika. Dan fungsi Arduino ini dibuat untuk memudahkan kita dalam melakukan prototyping, memprogram mikrokontroler, membuat alat-alat canggih berbasis mikrokontorler.

# Jenis - jenis arduino

1. **Arduino Uno**
![arduino uno saifulmqdr.ml](/images/arduino/uno.jpg)
    Jenis yang ini adalah yang paling banyak digunakan. Terutama untuk pemula sangat disarankan untuk menggunakan Arduino Uno. Dan banyak sekali referensi yang membahas Arduino Uno. Versi yang terakhir adalah Arduino Uno R3 (Revisi 3), menggunakan ATMEGA328 sebagai Microcontrollernya, memiliki 14 pin I/O digital dan 6 pin input analog. Untuk pemograman cukup menggunakan koneksi USB type A to To type B. Sama seperti yang digunakan pada USB printer.

2. **Arduino Due**
![arduino due saifulmqdr.ml](/images/arduino/due.jpg)
    Berbeda dengan saudaranya, Arduino Due tidak menggunakan ATMEGA, melainkan dengan chip yang lebih tinggi ARM Cortex CPU. Memiliki 54 I/O pin digital dan 12 pin input analog. Untuk pemogramannya menggunakan Micro USB, terdapat pada beberapa handphone.

3. **Arduino Mega**
![arduino mega saifulmqdr.ml](/images/arduino/mega.jpg)
    Mirip dengan Arduino Uno, sama-sama menggunakan USB type A to B untuk pemogramannya. Tetapi Arduino Mega, menggunakan Chip yang lebih tinggi ATMEGA2560. Dan tentu saja untuk Pin I/O Digital dan pin input Analognya lebih banyak dari Uno.

4. **Arduino Leonardo**
![arduino leonardo saifulmqdr.ml](/images/arduino/leonardo.jpg)
    Bisa dibilang Leonardo adalah saudara kembar dari Uno. Dari mulai jumlah pin I/O digital dan pin input Analognya sama. Hanya pada Leonardo menggunakan Micro USB untuk pemogramannya.

5. **Arduino Fio**
![arduino fio saifulmqdr.ml](/images/arduino/fio.jpg)
    Bentuknya lebih unik, terutama untuk socketnya. Walau jumlah pin I/O digital dan input analognya sama dengan uno dan leonardo, tapi Fio memiliki Socket XBee. XBee membuat Fio dapat dipakai untuk keperluan projek yang berhubungan dengan wireless.

6. **Arduino Lilypad**
![arduino lilypad saifulmqdr.ml](/images/arduino/lilypad.jpg)
    Bentuknya yang melingkar membuat Lilypad dapat dipakai untuk membuat projek unik. Seperti membuat amor iron man misalkan. Hanya versi lamanya menggunakan ATMEGA168, tapi masih cukup untuk membuat satu projek keren. Dengan 14 pin I/O digital, dan 6 pin input analognya.

7. **Arduino Nano**
![arduino nano saifulmqdr.ml](/images/arduino/nano.jpg)
    Sepertinya namanya, Nano yang berukulan kecil dan sangat sederhana ini, menyimpan banyak fasilitas. Sudah dilengkapi dengan FTDI untuk pemograman lewat Micro USB. 14 Pin I/O Digital, dan 8 Pin input Analog (lebih banyak dari Uno). Dan ada yang menggunakan ATMEGA168, atau ATMEGA328.

8. **Arduino Mini**
![arduino mini saifulmqdr.ml](/images/arduino/mini.jpg)
    Fasilitasnya sama dengan yang dimiliki Nano. Hanya tidak dilengkapi dengan Micro USB untuk pemograman. Dan ukurannya hanya 30 mm x 18 mm saja.

9. **Arduino Micro**
![arduino micro saifulmqdr.ml](/images/arduino/micro.jpg)
    Ukurannya lebih panjang dari Nano dan Mini. Karena memang fasilitasnya lebih banyak yaitu; memiliki 20 pin I/O digital dan 12 pin input analog.

10. **Arduino Ethernet**
![arduino ethernet saifulmqdr.ml](/images/arduino/ethernet.jpg)
    Ini arduino yang sudah dilengkapi dengan fasilitas ethernet. Membuat Arduino kamu dapat berhubungan melalui jaringan LAN pada komputer. Untuk fasilitas pada Pin I/O Digital dan Input Analognya sama dengan Uno.

11. **Arduino Esplora**
![arduino esplora saifulmqdr.ml](/images/arduino/esplora.jpg)
    Rekomendasi bagi kamu yang mau membuat gadget sepeti Smartphone, karena sudah dilengkapi dengan Joystick, button, dan sebagainya. Kamu hanya perlu tambahkan LCD, untuk lebih mempercantik Esplora.

12. **Arduino Robot.**
![arduino robot saifulmqdr.ml](/images/arduino/robot.png)
    Ini adalah paket komplit dari Arduino yang sudah berbentuk robot. Sudah dilengkapi dengan LCD, Speaker, Roda, Sensor Infrared, dan semua yang kamu butuhkan untuk robot sudah ada pada Arduino ini.


Bagaimana, Apa sudah ada gambaran tentang arduino?. Ok Saya anggap sudah :v
Pada artikel kali ini dan seterusnya, saya akan menggunakan arduino uno sebagai bahan praktek membuat projeck simple. Mengapa pake arduino uno? Ya karna arduino uno saya rasa mudah didapat, mudah digunakan dan banyak artikel dan tutorial yg menggunakan arduino uno ini. Jadi rekomend banged buat para beginder.

# Ada apa aja didalam board arduino?

Ada banyak varian jenis board arduino yg dapat digunakan beberapa board ada yang terlihat sedikit berbeda tetapi hampir semua komponen utama sama. Dibawah ini adalah board arduino uno dan saya akan mencoba menjelaskan apa aja yg ada didalamnya.

![board arduino uno saifulmqdr.ml](/images/arduino/board_uno.jpg)

### Power (USB / Barrel Jack)

Setiap Arduino memiliki jalur yang akan dihubungkan dengan sumber tenaga/tegangan. Arduino UNO dapat diberi tegangan melalui USB (1) dapat berasal dari komputer, power bank atau berasal dari power supply melalui barrel jack (2). Koneksi kabel USB juga berfungsi untuk jalur pemograman ke board Arduino.

Warning: Jangan menggunakan power supply yang tegangannya lebih dari 20 Volt, karena dapat merusak board Arduino karena overpower. Tegangan yang dizinkan untuk Arduino adalah 6 - 12 Volt.

### Pin (5V, 3.3V, GND, Analog, Digital, PWM, AREF)

Pin pada Arduino adalah tempat dimana untuk menyambungkan kabel antara pin Arduino dengan perangkat-perangkat input/output (biasanya menghubungkan dengan rangakain project pada breadboard). Pin Arduino biasanya berupa female header sehingga untuk mendapatkan koneksi dari pin Arduino hanya cukup colokan kabel ke dalam lubang pin header tersebut. Terdapat beberapa pin pada Arduino dengan fungsi yang berbeda-beda, masing-masing pin diberi label sesuai nama dan fungsinya pada PCB.

— GND (3): Kependekan dari 'Ground'. Terdapat beberapa pin ground dan semuanya dapat digunakan.

— 5V (4) & 3.3V (5): 5V pin memberikan supply tegangan 5 volt, dan 3.3V pin memberikan supply tegangan 3.3 volt. Kebanyakan arduino pake tegangan 5 atau 3.3 volt

— Analog (6): Pin yang berada di bawah tulisan 'Analog In' (A0 sampai A5 pada Arduino UNO) adalah pin Analog Input. Pin ini dapat membaca sinyal dari sensor analog (seperti sensor suhu) dan mengkonversinya kedalam nilai digital yang dapat kita baca.

— Digital (7): Terletak disisi lain dari analog pin terdapat pin digital (0 sampai 13 pada UNO). Pin ini dapat difungsikan sebagai digital input (seperti memberitahukan apabila button dipencet) dan digital output (seperti menyalakan sebuah LED).

— PWM (8): Kalian bisa melihat simbol (~) pada beberapa pin digital (3, 5, 6, 7, 9, 10, dan 11 pada UNO). Pin ini berfungsi sebagai pin digital biasanya, tapi bisa digunain juga untuk Pulse-Width Modulation (PWM), sederhananya pin ini dapat mengeluarkan keluaran tegangan Analog.

— AREF (9): Singkatan dari Analog Reference. Pin ini digunakan untuk mengatur tegangan referensi external (antara 0 dan 5 volt) sebagai batas untuk pin analog input.

### Tombol Reset

Kek komputer pada umumnya, Arduino punya tombol reset (10). Menekan tombol ini akan menghubungkan pin reset dengan ground dan merestart semua kode program yang ada di dalam Arduino. Reset ini akan sangat membantu jika kode tidak berjalan berulang-ulang, tapi kamu ingin menjalankannya beberapa kali.

### Power LED Indicator

Tepat di bawah dan di sebelah kanan kata "UNO" di board Arduino, ada LED kecil di samping kata 'ON' (11). LED ini harus menyala setiap kali Anda memasukkan Arduino Anda ke sumber tegangan. Jika lampu ini tidak menyala, ada kemungkinan ada sesuatu yang salah.

### TX RX LED

TX adalah singkatan dari transmit, RX adalah singkatan dari receive. Kata ini cukup familiar dalam istilah elektronik untuk menunjukkan pin sebagai komunikasi serial. Dalam board Arduino terdapat dua tempat tulisan TX dan RX - pertama pada pin digital 0 dan 1, dan yang kedua di samping indikator LED TX dan RX (12). LED ini akan memberi kita beberapa indikasi visual setiap kali Arduino menerima atau mentransmisikan data (seperti saat kita memasukan program baru ke board Arduino).

### IC Utama

Berwarna hitam terdapat banyak kaki logam disampingnya adalah IC, atau Integrated Circuit (13). Anggap saja itu sebagai otaknya Arduino. IC utama pada Arduino UNO berbeda dengan jenis board Arduino lainnya tapi biasanya merupakan IC keluarga ATmega yang diproduksi oleh perusahaan ATMEL. Untuk mengetahui jenis IC yang dipakai bisa ditemukan secara tertulis disisi atas IC. Jika Anda ingin tahu lebih banyak tentang perbedaan antara IC tersebut, dapat dilihat pada datasheet.

### Voltage Regulator

Regulator tegangan (14) berfungsi untuk membatasi jumlah tegangan yang masuk ke board Arduino. Anggap saja itu sebagai semacam gatekeeper; ini akan menghilangkan tegangan lebih yang mungkin membahayakan sirkuit. Tentu saja, ini memiliki batas, jadijangan menghubungkan Arduino Anda dengan yang lebih besar dari 20 volt.

Buat yg mau beli, tapi gk tau bli d mn. Cek aja toko online kek Lazada, shopi, tokopedia. Kalo gw sih d lazada karna bisa cod :v. Kalo klean gk punya akun onlenshop kalian bisa langsung beli ke toko cnc store bandung.

Ok mungkin cukup sekian, semoga bermanfa'at, sampai jumpa d artikel berikutnya 😐
