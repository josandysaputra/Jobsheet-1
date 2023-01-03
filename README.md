# Jobsheet-1

DASAR PEMROGRAMAN ESP32 UNTUK PEMROSESAN DATA INPUT/OUTPUT ANALOG DAN DIGITAL
TUJUAN
  1) Mahasiswa dapat memahami dan mengoperasikan GPIO pada ESP32.
  2) Mahasiswa dapat memahami dan melakukan pengolahan data untuk 
  input/output analog dan digital.
  3) Mahasiswa dapat melakukan optimalisasi pembacaan sensor analog 
  menggunakan metode regresi linear.
  
ALAT DAN BAHAN
  1) ESP32
  2) Breadboard
  3) Multimeter
  4) Kabel jumper
  5) Potensiometer 10k Ohm (1)
  6) Sensor Capacitive Soil Moisture
  7) LED (5) dan Push Button (3)
  8) Resistor 330,1K, 10K Ohm (3)
  
  ESP-32 adalah mikrokontroler yang dikenalkan oleh Espressif System merupakan penerus dari mikrokontroler ESP8266. Pada mikrokontroler ini sudah 
tersedia modul WiFi dalam chip sehingga sangat mendukung untuk membuat sistem aplikasi Internet of Things. 
  Perbedaan antara ESP32 dengan ESP8266 adalah pada bagian prosesornya. ESP32 sudah Dual-Core 32 bit, jelas lebih cepat ESP32 secara kinerja. Selain itu modul ini juga mempunyai bluetooth, satu fitur yang tidak ada di ESP8266.
  
  
A. GPIO
1. Buka program example blink, kemudian modifikasi dan buat agar LED dapat melakukan blink dengan interval 100ms, 1 detik, 2 detik dan 3 detik sekali. 
Setelah itu, buatlah program agar LED dapat blink 1 detik sekali menggunakan timer milis.

https://user-images.githubusercontent.com/121847212/210306827-60d72c68-34b0-45fa-bf70-755d52f8cbf3.MOV



2. Tambahkan 1 LED dan 1 push button pada rangkaian, kemudian kembangkan program agar ketika push button ke-2 ditekan, LED akan melakukan blink setiap 500 ms sekali.


https://user-images.githubusercontent.com/121847212/210308481-3c9713b9-18e4-44c5-853c-df97d162a04d.mp4


3. Tambahkan 3 LED dan 1 push button pada rangkaian, kemudian kembangkan program agar ketuka push button ke-3 ditekan, LED akan menyala menjadi running led (menyala      bergantian dari kiri ke kanan).


https://user-images.githubusercontent.com/121847212/210308512-54364846-5586-44e7-aaa9-409f717dc2ab.MOV



B. PWM
1. Upload program tersebut, kemudian amati dan analisis apa yang terjadi serta 
  dokumentasikan hasilnya


https://user-images.githubusercontent.com/121847212/210307835-408db723-baf2-4e47-83df-974df03db75a.MOV

2. Upload program tersebut, kemudian amati dan analisis apa yang terjadi serta dokumentasikan hasilnya.


https://user-images.githubusercontent.com/121847212/210307886-b86ccdf4-b104-494c-9cf6-200645754796.MOV


C. ADC dan DAC
1. Buatlah program seperti pada script Putar potensiometer secara perlahan agar mendapatkan nilai 0 hingga 4095 pada tampilan serial monitor.


https://user-images.githubusercontent.com/121847212/210309332-18b34c5e-48ef-4597-9ebc-d23a9f863a14.MOV


2. Buatlah program seperti pada script berikut ini.Tambahkan LED pada GPIO 5 kemudian upload program, kemudian putar potensiometer dari nilai terendah hingga 
  nilai tertinggi.


https://user-images.githubusercontent.com/121847212/210309890-8a0f78eb-2158-4dce-acfc-f276441f0a4c.mp4



D. Simulasi Pemrosesan Data Menggunakan Regresi Linier
1. Buatlah dan upload script program,Masukkan sensor pada sampel tanah 1-3. Catat hasil pembacaan sensor dan 3 Way Meter pada masing-masing sampel tanah Ukur tegangan output sensor pada pin Aout (A) menggunakan multimeter kemudian catat hasilnya.

2. Upload program berikut pada ESP32 Catat keluaran dari vs, Masukkan semua data pada tabel Excel menggunakan format berikut Buatlah scatter chart dengan sumbu X = Vs dan sumbu Y = 3 Way Meter. Klik kanan line pada scatter chart, kemudian pilih add trendline. Kemudian pada format trendline, atur trendline option = linear, checklist pada Display Equaiton on Chart dan Display R-squared value on Chart, Masukkan persamaan yang dihasilkan grafik ke dalam program Arduino.Ganti variabel a dan b dengan nilai pada persamaan yang dihasilkan dokumentasikan hasilnya, serta buatlah analisis dan kesimpulannya.


