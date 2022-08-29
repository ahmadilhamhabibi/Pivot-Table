


### **Pivot Table dan Interaktif Dashboard Sederhana untuk Data Analyst**

Diantara tugas seorang Data Analyst adalah mengolah dan menyampaikan informasi dari suatu data mentah menjadi sebuah informasi utuh yang bisa memberikan insight kepada pembaca. Ketika melakukan analisis data dengan menggunakan spreadsheet, kita bisa memanfaatkan fitur **PivotTable** dan **PivotChart** untuk membuat dashboard sederhana. Pada kesempatan kali ini saya akan membahas tentang bagaimana membuat PivotTable hingga menjadi dashboard. Tulisan kali ini akan membahas tentang:

 1.  **Definisi Pivot Table**
Pivot Table adalah alat canggih untuk menghitung, meringkas, dan menganalisis data yang memungkinkan Anda melihat perbandingan, pola, dan tren dalam data Anda (support.microsoft). Pivot Table merupakan fitur yang sudah ada dalam Microsoft Excel, tetapi masih banyak orang yang belum memanfaatkannya dengan maksimal. Salah satu keunggulan Pivot Table adalah untuk memudahkan pengambilan informasi secara cepat dari kumpulan data yang jumlahnya besar.

 2.  **Import Data**
Langkah pertama untuk membuat Pivot Tabel adalah dengan memasukkan (_import_) data ke dalam worksheet.

 -   Pada menu bar pilih **Data**
 -   Pada bagian pojok kiri atas akan ada pilihan **Get & Transform Data**
 -   Klik **Get Data** maka akan muncul beberapa pilihan source data
 ![ImportData](https://github.com/ahmadilhamhabibi/Pivot-Table/blob/6a1adbbfc64dd77233e92663631f1f28b8dbf38b/Images/2.1.ImportData.png)

 3.  **Persiapan untuk Analisis Data**
Setelah memilih data yang akan diinput, akan muncul pilihan untuk langsung meng-_load_ data atau mentransformasikan data terlebih dahulu. Pada proses ini menggunakan fitur **Power Query** yang bisa digunakan untuk membersihkan data, seperti: menentukan delimiter, data type, hapus duplikat, hapus kolom, dan proses pembersihan data lainnya. Setelah selesai pilih **close and load** pada pojok kiri atas.
![ImportData](https://github.com/ahmadilhamhabibi/Pivot-Table/blob/6a1adbbfc64dd77233e92663631f1f28b8dbf38b/Images/3.1.LoadData.png)

 4. **Membuat dan Memanipulasi Pivot Table**
 Banyak cara untuk membuat Pivot Table. Pada tahap persiapan kita bisa langsung membuatnya setelah membersihkan data. Pilih **Close and Load to** kemudian pilih **PivotTable Report** untuk langsung membuat Pivot Table.
 Jika langsung memilih **Close and Load** maka akan muncul tabel pada workbook di Ms Excel. Pada menu bar pilih **Insert => Pivot Table**, pilih tabel yang akan dijadikan Pivot Table serta pilih destinasi untuk hasil Pivot Table yang akan dibuat.
 Setelah klik OK, akan muncul worksheet baru untuk membuat Pivot Table. Akan ada dua tampilan bar tambahan di atas, yaitu: **PivotTable Analyze** dan **Design**.
Pada kolom sebelah kanan kita bisa mengedit **PivotTable Fields** yang berisi kolom-kolom pada tabel. Ketika menjadi Pivot Table kolom-kolom ini menjadi satu element yang bisa kita sesuaikan posisinya menjadi kolom, baris, nilai, atau filter. Bisa dibilang **PivotTable Fields** adalah bagian terpenting ketika membuat Pivot Table.
 ![Pivot Table](https://github.com/ahmadilhamhabibi/Pivot-Table/blob/6a1adbbfc64dd77233e92663631f1f28b8dbf38b/Images/4.3.PivotTable.png)
 5.  **Value Field Setting**
Pada contoh sebelumnya di kotak **value** berisi **Sum of Sales** dan **Sum of Profit** karena _setelan pabrik_ pada kotak **value** adalah **sum**, atau menjumlahkan nilai dari data. Kita bisa menyesuaikan kotak **value** ini dengan cara klik pada kolom yang ingin diubah (misalnya: profit), **klik kanan**, kemudian pilih **Value Field Setting**.
pada kolom **Summarize Value By** kita bisa melihat pilihan lainnya seperti **Count, Average, Min, Max,** dan lain-lain. Berikut adalah contoh untuk **summarize velue** dengan nilai minimal, maksimal, dan rata-rata.
Selain **Summarize Value By**, pada **Value Field Setting** juga terdapat pilihan **Show Value As** yang berfungsi untuk menampilkan nilai sesuai dengan paramater tertentu. Misalnya **% of Grand total, % of colums, Running total** dan sebagainya. Berikut contoh Provit yang ditampilkan sebagai **% of Grand total** dan **Running total.**
![ValueFieldSetting](https://github.com/ahmadilhamhabibi/Pivot-Table/blob/6a1adbbfc64dd77233e92663631f1f28b8dbf38b/Images/5.2.ValueFieldSetting1.png)

 6. **Sorting dan Filtering**
Sorting dan Filtering sangat berguna untuk memudahkan memindai data, mengurutkan data, serta mengatur data mana saja yang ingin ditampilkan. Sorting dan Filtering berguna untuk memudahkan kerja Data Analyst ketika kita beradapan dengan data yang banyak.
Sorting berguna untuk mengurutkan data. Pada **Row Labels** terdapat kotak putih disebelah kanan yang bisa digunakan untuk Sorting dan Filtering data. Selain itu, bisa juga dengan cara klik kanan pada data terus pilih **Sort**. Data tipe teks bisa diurutkan sesuai abjad (A-Z) atau kebalikannya (Z-A).
Data Numerik bisa diurutkan dari nilai tertinggi atau terendah. Hal ini sangat berguna ketika membuat report. Misalnya untuk melihat _product_ yang paling laris di pasaran, siapa _sales person_ yang paling banyak penjualannya, dan lain sebagainya. Berikut contoh sorting berdasarkan nilai **Sum of Sales** tertinggi.
Filtering berguna untuk menentukan data mana saja yang ingin ditampilkan. Misalnya ingin menampilkan label tertentu atau nilai tertentu. Filter berdasarkan nilai bisa digunakan untuk melihat 10(**n)** nilai teratas atau 10(**n)** nilai terendah. Misalnya ingin melihat tiga negara dengan Profit tertinggi. Dalam hal ini bisa memanfaatkan fitur Filter.
![FilteringNumerik](https://github.com/ahmadilhamhabibi/Pivot-Table/blob/6a1adbbfc64dd77233e92663631f1f28b8dbf38b/Images/6.4.FilteringDataNumerik.png)

 7.  **Berinteraksi dengan Pivot Table dengan Slicer dan Timeline**
Fungsi Slicer dan Timeline hampir sama dengan filter, yaitu untuk menampilkan data sesuai degan kriteria tertentu. Bedanya, Slicer dan Timeline memiliki _dialog box_ yang bisa diubah sesuai keinginan. Slicer dan Timeline sangat berguna untuk membuat **_Interactive Dashboard_**.
Pada menu bar **PivotTable Analyze** terdapat pilihan untuk menambahkan **Slicer** dan **Timeline.** Slicer berfungsi untuk memfilter data kategorikal, sedangkan Timeline khusus untuk memfilter data tipe _date_.
Setelah muncul dialog box, kita bisa berinteraksi dengan Pivot Table dengan memilih data mana saja yang akan ditampilkan. Bisa memilih satu data atau lebih. Khusus **Timeline**, kita bisa memilih bulan, quarter, atau tahun sesuai dengan kebutuhan.
Setidaknya ada dua hal yang perlu diperhatikan ketika menggunakan Slicer.
![SlicerAndTimeline](https://github.com/ahmadilhamhabibi/Pivot-Table/blob/6a1adbbfc64dd77233e92663631f1f28b8dbf38b/Images/7.1.SlicerAndTimeline.png)
 -   Pertama, matikan _Autofit Column Width_ agar lebar kolom tidak berubah-ubah. Pada menu bar **PivotTable Analyze** pilih **PivotTable** option kemudian hilangkan centang pada _Autofit Column Width._
 -   Kedua pastikan Slicer terkoneksi dengan tabel yang ingin ditampilkan. Karena Slicer hanya akan berkerja kepada tabel dan chart yang sudah terkoneksi dengan Slicer. Misalnya pada dashboard ada chart yang belum terkoneksi dengan Slicer, maka chart ini tidak akan berubah ketika kita mengubah Slicer. Pada bar **Slicer** pilih **Report Connections**, kemudian centang tabel yang akan diperlukan.
 
 8.  **Pivot Chart**
 Mata manusia lebih mudah menangkap informasi dalam bentuk gambar (_Chart_) daripada tabel. Itulah sebabnya dalam membuat laporan sering kali ditampilkan dalam bertuk gambar (dashboard). Tujuannya untuk mempermudah penyampaian informasi.
Proses mengubah data menjadi gambar disebut Visualisasi Data (_Data Visualization_). Visualisasi data merupakan aspek yang sangat penting dalam proses analisis data. Karena pentingnya proses _Data Visualization,_ dalam banyak kursus Data Analyst sampai dibahas dalam bab tersendiri.
Saat menganalisis data menggunakan Spreadsheet, utamanya Pivot Table, kita bisa memanfaatkan fitur **Pivot Chart**. Caranya, letakkan pointer pada Pivot Table. Pada bar **PivotTable Analyze** pilih **PivotChart**.
Kemudian akan ada pilihan chart yang bisa digunakan untuk memvisualisasikan data. Diantarnya:
   - Column Chart
   -   Line Chart
   -   Pie Chart
   -   Bar Chart
   -   Area Chart
   -   Scatter Chart
   -   Map Chart
   -   dan lain-lain
 Kali ini saya akan memberikan contoh column chart, line chart, pie chart (doughnut chart), dan bar chart. Untuk pemilihan chart dan fungsikan akan dibahas dalam tulisan yang lain.
 ![Column](https://github.com/ahmadilhamhabibi/Pivot-Table/blob/6a1adbbfc64dd77233e92663631f1f28b8dbf38b/Images/8.2.ColumnChart.png)
 ![Bar](https://github.com/ahmadilhamhabibi/Pivot-Table/blob/6a1adbbfc64dd77233e92663631f1f28b8dbf38b/Images/8.3.BarChart.png)
 ![Pie](https://github.com/ahmadilhamhabibi/Pivot-Table/blob/6a1adbbfc64dd77233e92663631f1f28b8dbf38b/Images/8.4.PieChart.png)
 ![Line](https://github.com/ahmadilhamhabibi/Pivot-Table/blob/6a1adbbfc64dd77233e92663631f1f28b8dbf38b/Images/8.5.LineChart.png)

 9. **Interaktif Dashboard Sederhana**
Dengan memanfaatkan **Pivot Chart** dan **Slicer** kita bisa membuat interaktif dashboard. Kali ini saya akan memberikan contoh dashboard sederhana dengan memanfaatkan empat gambar diatas.
Salin keempat chart ke dalam satu worksheet. Buat dua slicer berisi **Year** dan **Product**. Pastikan semua tabel dan chart terkoneksi dengan Slicer. Kemudian atur layout sesuai keinginan.
Berikut contoh interaktif dashboard sederhana yang telah saya buat:
![Dashboard](https://github.com/ahmadilhamhabibi/Pivot-Table/blob/6a1adbbfc64dd77233e92663631f1f28b8dbf38b/Images/9.1.InteraktifDashboard.png)
Interaktif dashboard bisa diubah dengan memanipulasi Slicer. Misalnya saya ingin melihat data penjualan dari 3 produk (Vermont, Luxe, Mandarin) pada tahun 2019. Maka tampilan dashboard akan menjadi seperti dibawah ini:
![InteraktifDashbiard](https://github.com/ahmadilhamhabibi/Pivot-Table/blob/6a1adbbfc64dd77233e92663631f1f28b8dbf38b/Images/9.2.InteraktifDashboard.png)

Demikian catatan saya tentang Pivot Table dan Interaktif Dashboard Sederhana. Terima kasih telah membaca. Sila dibookmark dan dibagikan. Semoga bermanfaat. 

