# 🛒 Sales Exploratory Data Analyst ( Mini Task )

## 📍Introduction
Dataset yang digunakan merupakan dataset dummy yang berisi data penjualan barang dengan kategori Apparel, Equipment, dan Footwear. Dataset ini terdiri dari 1000 data.

Spreadsheet Link : [Sales Exploratory Data Analyst](https://docs.google.com/spreadsheets/d/1b12K_JxBO1D9RxYAJQkUncD0zM5rKDK5rYYvgnGXozc/edit?usp=sharing)

Pada Readme File ini akan dijelaskan
1. Objectives
2. Analysis Data (Data Preprocessing, Exploratory Data Analysis, Hasil EDA)
3. Kesimpulan

## 🔎 Objectives
 1. Bagaimana Trend Penjualan dan Pendapatan produk (total) setiap bulan?
 2. Bagaimana persentase penjualan produk berdasarkan kategori produk?
 3. Bagaimana trend penjualan produk berdasarkan jenis produk ?
 4. Bagaimana pendapatan dari penjualan produk berdasarkan kategori produk?

## Analysis Data

### 🔁 Data Preprocessing
1. Memisahkan Kode Penjualan Produk dengan Nama Negara menggunakan fungsi LEFT dan MID
2. Memisahkan Kategori Produk dan Jenis" pada setiap kategori dengan feature split text to column
3. Mengubah format setiap kolom yang sesuai
4. Mengurutkan data berdasarkan bulannya

### 🖥️ Exploratory Data Analysis
1. Menggunakan Pivot Table untuk mendapatkan return table sesuai objective yang di inginkan.
2. Membuat Analisa deskriptif pada setiap objective.
3. Menampilkan dalam bentuk chart untuk memahami hasilnya lebih jelas.
4. Menganalisis pendistribusian data dan nilai skewnessnya.
5. Membuat box plot untuk mengetahui pemusatan data.
   
### 🎯 Hasil
### 📈 Trend Penjualan dan Pendapatan setiap bulan

![image](https://github.com/user-attachments/assets/39340be7-7e6b-4964-97b6-dcbb0cbeea00)

  
### 📈 Penjualan dan Pendapatan berdasarkan kategori

  Visualisasi :

  ![image](https://github.com/user-attachments/assets/184f7593-bf3a-4327-8582-e41c8a111727)
  ![image](https://github.com/user-attachments/assets/394d9388-3749-4071-a858-ba104931d1c0)

Insight :
- Terlihat pada pie chart dari tabel frekuensi menunjukan bahwa kategori produk dengan **penjualan terbanyak dan pendapatan tertinggi** yaitu **kategori Equipment**. Sedangkan **kategori Footwear memiliki penjualan dan pendapatan paling rendah**. Padahal **Kategori Footwear memiliki jenis produk yang lebih banyak** dibandingkan dengan kategori lainnya.
- Selain itu, mesikipun **kategori Equipment** memiliki predikat sebagai **kategori** dengan **penjualan terbanyak dan pendapatan tertinggi**, **Jenis Produk** dengan **penjualan terbanyak dan pendapatan tertinggi** jatuh kepada **jenis produk Outerwear pada Kategori Apparel**. 

  | **KATEGORI PRODUK** | **JENIS PRODUK** | **UNIT TERJUAL** | **PENDAPATAN ($)** |
  |---------------------|------------------|------------------:|--------------------:|
  | **Apparel**         | Outerwear        | 3,738,117         | $718,926,880        |
  |                     | Performance      | 3,009,477         | $497,096,740        |
  |                     | Tops             | 3,164,500         | $513,052,500        |
  |                     | **Apparel Total**| **9,912,094**     | **$1,729,076,120**  |
  | **Equipment**       | Accessories      | 3,638,389         | $629,192,700        |
  |                     | Bags             | 3,354,567         | $593,442,370        |
  |                     | Socks            | 2,998,893         | $554,690,320        |
  |                     | **Equipment Total**| **9,991,849**   | **$1,777,325,390**  |
  | **Footwear**        | Basketball       | 1,734,235         | $277,342,380        |
  |                     | Cricket          | 1,897,998         | $384,372,340        |
  |                     | Football         | 1,704,349         | $303,153,710        |
  |                     | Lifestyle        | 1,779,075         | $314,578,270        |
  |                     | Running          | 1,479,351         | $253,727,970        |
  |                     | **Footwear Total**| **8,595,008**    | **$1,533,174,010**  |
  |                     | **Grand Total**  | **28,498,951**    | **$5,039,576,410**  |


      
### 📈 Pendapatan setiap jenis produk perbulan beserta analisis deskriptifnya.

Distribusi Data Pendapatan (semua kategori) :
---
![image](https://github.com/user-attachments/assets/6520a839-a79a-4ee4-b419-2c97ee396770)

Pada visualisasi histogram disamping menunjukan bahwa sebaran **data pendapatan tidak normal** (puncak dikiri, miring ke kanan) dan memiliki **skewness positif**. Hal ini berarti distribusi pendapatan penjualan produk **paling banyak terdistribusi pada pendapatan terendah**. 

Pada detail histogram di bawah menunjukan bahwa jenis produk pada kategori **Footwear memiliki distribusi yang tidak normal**. **Produk Cricket** dan **Running** memiliki **Skewness yang cenderung besar**.


### 1. Accessories
----

| BULAN     | PENDAPATAN ($) |
|-----------|----------------|
| April     | $78,123,000    |
| August    | $35,487,410    |
| December  | $45,764,610    |
| February  | $57,630,640    |
| January   | $49,569,970    |
| July      | $42,856,700    |
| June      | $46,973,390    |
| March     | $31,972,080    |
| May       | $65,058,880    |
| November  | $82,041,600    |
| October   | $24,374,840    |
| September | $69,339,580    |
| **Total**: | $629,192,700 |

Analisa Deskriptif Pendapatan Kategori Accessoris : 
---
| Statistik           | Nilai          |
|---------------------|----------------|
| Mean                | 52,432,725     |
| Standard Error      | 5,277,271.08   |
| Median              | 48,271,680     |
| Mode                | 82,041,600     |
| Standard Deviation  | 18,281,003.27  |
| Sample Variance     | 334,195,080,635,282 |
| Kurtosis            | -0.9282460603  |
| Skewness            | 0.2324593283   |
| Range               | 57,666,760     |
| Minimum             | 24,374,840     |
| Maximum             | 82,041,600     |
| Sum                 | 629,192,700    |
| Count               | 12             |

Distribusi Data Pendapatan Accesoris :
---

![image](https://github.com/user-attachments/assets/c928e1b0-21fb-431e-8138-eac110a4f8fb)


### 2. Bags
---

| BULAN     | PENDAPATAN ($) |
|-----------|----------------|
| April     | $42,278,210    |
| August    | $24,905,100    |
| December  | $79,155,950    |
| February  | $53,130,170    |
| January   | $75,179,540    |
| July      | $44,847,280    |
| June      | $37,192,180    |
| March     | $28,004,780    |
| May       | $64,069,970    |
| November  | $52,104,140    |
| October   | $61,723,030    |
| September | $30,852,020    |
|**Total**: | $593,442,370   |


Analisa Deskriptif Pendapatan Kategori Bags :
---
| Statistik           | Nilai              |
|---------------------|--------------------|
| Mean                | 49,453,530.83      |
| Standard Error      | 5,193,614.69       |
| Median              | 48,475,710         |
| Mode                | 79,155,950         |
| Standard Deviation  | 17,991,209.05      |
| Sample Variance     | 323,683,603,114,245|
| Kurtosis            | -1.017629201       |
| Skewness            | 0.278386589        |
| Range               | 54,250,850         |
| Minimum             | 24,905,100         |
| Maximum             | 79,155,950         |
| Sum                 | 593,442,370        |
| Count               | 12                 |

Distribusi Data Pendapatan Bags :
---
![image](https://github.com/user-attachments/assets/e0d1152d-5571-4a7e-a8af-ee3b9a9cbf14)


### 3. Basketball

| BULAN     | PENDAPATAN ($) |
|-----------|----------------|
| April     | $26,754,770    |
| August    | $19,464,120    |
| December  | $47,239,280    |
| February  | $26,506,040    |
| January   | $18,790,920    |
| July      | $7,331,390     |
| June      | $13,405,680    |
| March     | $19,846,420    |
| May       | $38,870,760    |
| November  | $5,571,940     |
| October   | $16,559,390    |
| September | $37,001,670    |
| **Total**: | $277,342,380 |

Analisa Deskriptif Pendapatan Kategori Basketball :
---
| Statistik           | Nilai              |
|---------------------|--------------------|
| Mean                | 23,111,865         |
| Standard Error      | 3,676,965.41       |
| Median              | 19,655,270         |
| Mode                | 47,239,280         |
| Standard Deviation  | 12,737,381.80      |
| Sample Variance     | 162,240,895,122,555|
| Kurtosis            | -0.4049491978      |
| Skewness            | 0.5300327301       |
| Range               | 41,667,340         |
| Minimum             | 5,571,940          |
| Maximum             | 47,239,280         |
| Sum                 | 277,342,380        |
| Count               | 12                 |

Distribusi Data Pendapatan Basketball :
---
![image](https://github.com/user-attachments/assets/7c7e5d1e-e8fb-42f4-bff5-6bac1ce36adf)

### 4. Cricket

| BULAN     | PENDAPATAN ($) |
|-----------|----------------|
| April     | $29,756,730    |
| August    | $12,186,750    |
| December  | $79,509,210    |
| February  | $26,335,720    |
| January   | $34,709,770    |
| July      | $45,007,320    |
| June      | $41,105,090    |
| March     | $27,253,850    |
| May       | $7,373,020     |
| November  | $28,878,500    |
| October   | $14,996,490    |
| September | $37,259,890    |
|**Total**: | $384,372,340 |

Analisa Deskriptif Pendapatan Kategori Cricket :
---

| Statistik           | Nilai              |
|---------------------|--------------------|
| Mean                | 32,031,028.33      |
| Standard Error      | 5,436,809.32       |
| Median              | 29,317,615         |
| Mode                | 79,509,210         |
| Standard Deviation  | 18,833,659.95      |
| Sample Variance     | 354,706,747,052,433|
| Kurtosis            | 3.140423348        |
| Skewness            | 1.339571298        |
| Range               | 72,136,190         |
| Minimum             | 7,373,020          |
| Maximum             | 79,509,210         |
| Sum                 | 384,372,340        |
| Count               | 12                 |

Distribusi Data Pendapatan Kategori Cricket :
---
![image](https://github.com/user-attachments/assets/cbbab6ed-bee7-4c67-bb56-63b9eb83479b)



### 5. Football

| BULAN     | PENDAPATAN ($) |
|-----------|----------------|
| April     | $9,394,680     |
| August    | $22,129,700    |
| December  | $42,133,300    |
| February  | $30,592,490    |
| January   | $23,591,510    |
| July      | $40,048,860    |
| June      | $21,479,820    |
| March     | $27,355,030    |
| May       | $16,571,840    |
| November  | $12,794,410    |
| October   | $22,460,830    |
| September | $34,601,240    |
| **Total**: | $303,153,710 |

Analisa Deskriptif Pendapatan Kategori Football :
---
| Statistik           | Nilai              |
|---------------------|--------------------|
| Mean                | 25,262,809.17      |
| Standard Error      | 2,939,791.13       |
| Median              | 23,026,170         |
| Mode                | 42,133,300         |
| Standard Deviation  | 10,183,735.21      |
| Sample Variance     | 103,708,462,796,245|
| Kurtosis            | -0.650764606       |
| Skewness            | 0.2383159333       |
| Range               | 32,738,620         |
| Minimum             | 9,394,680          |
| Maximum             | 42,133,300         |
| Sum                 | 303,153,710        |
| Count               | 12                 |

Distribusi Data Pendapatan Football :
---
![image](https://github.com/user-attachments/assets/6d1730a6-8443-4862-8c85-040f0bd613c3)

### 6. Lifestyle

| BULAN     | PENDAPATAN ($) |
|-----------|----------------|
| April     | $4,518,700     |
| August    | $25,318,050    |
| December  | $29,563,360    |
| February  | $50,674,230    |
| January   | $13,674,650    |
| July      | $40,064,840    |
| June      | $8,887,840     |
| March     | $33,001,760    |
| May       | $29,932,470    |
| November  | $18,616,850    |
| October   | $32,758,610    |
| September | $27,567,360    |
| **Total**: | $314,578,720 |

Analisa Deskriptif Pendapatan Kategori Lifestyle :
---

| Statistik          | Nilai             |
|--------------------|-------------------|
| Mean               | 26,214,893.33     |
| Standard Error     | 3,786,506.75      |
| Median             | 28,565,360        |
| Mode               | 50,674,230        |
| Standard Deviation | 13,116,844.16     |
| Sample Variance    | 172,051,600,624,988 |
| Kurtosis           | -0.1007           |
| Skewness           | 0.0071            |
| Range              | 46,155,530        |
| Minimum            | 4,518,700         |
| Maximum            | 50,674,230        |
| Sum                | 314,578,720       |
| Count              | 12                |

Distribusi Data Pendapatan Kategori Lifestyle :
---
![image](https://github.com/user-attachments/assets/e3bf5292-f2c9-4f04-aa4b-8532837b3007)


### 7. Outerwear

| BULAN     | PENDAPATAN ($) |
|-----------|----------------|
| April     | $70,479,420    |
| August    | $29,874,900    |
| December  | $53,653,550    |
| February  | $40,992,200    |
| January   | $82,104,060    |
| July      | $65,552,610    |
| June      | $86,399,680    |
| March     | $66,662,360    |
| May       | $70,761,130    |
| November  | $62,384,010    |
| October   | $54,042,450    |
| September | $36,020,510    |
| **Total**: |  $718,926,880 |

Analisa Deskriptif Pendapatan Kategori Outerwear :
---
| Statistik          | Nilai            |
|--------------------|------------------|
| Mean               | 59,910,573.33    |
| Standard Error     | 5,083,814.69     |
| Median             | 63,968,310       |
| Mode               | 86,399,680       |
| Standard Deviation | 17,610,850.67    |
| Sample Variance    | 310,142,061,166,515 |
| Kurtosis           | -0.6999          |
| Skewness           | -0.3090          |
| Range              | 56,524,780       |
| Minimum            | 29,874,900       |
| Maximum            | 86,399,680       |
| Sum                | 718,926,880      |
| Count              | 12               |

Distribusi Data Pendapatan Kategori Outerwear :
---
![image](https://github.com/user-attachments/assets/d4d70c9f-a883-40eb-aaae-396b36d0044e)

### 8. Performance

| BULAN     | PENDAPATAN ($) |
|-----------|----------------|
| April     | $45,300,930    |
| August    | $40,543,990    |
| December  | $36,285,330    |
| February  | $24,456,120    |
| January   | $36,049,520    |
| July      | $59,605,990    |
| June      | $47,464,400    |
| March     | $33,495,080    |
| May       | $25,411,820    |
| November  | $65,196,610    |
| October   | $57,646,520    |
| September | $25,640,430    |
| **Total**: | $497,096,740 |

Analisa Deskriptif Pendapatan Kategori Performance :
---
| Statistik          | Nilai               |
|--------------------|---------------------|
| Mean               | 41,424,728.33       |
| Standard Error     | 4,010,178.35        |
| Median             | 38,414,660          |
| Mode               | 65,196,610          |
| Standard Deviation | 13,891,665.29       |
| Sample Variance    | 192,978,364,576,306 |
| Kurtosis           | -1.0053             |
| Skewness           | 0.4182              |
| Range              | 40,740,490          |
| Minimum            | 24,456,120          |
| Maximum            | 65,196,610          |
| Sum                | 497,096,740         |
| Count              | 12                  |

Distribusi Data Pendapatan Kategori Performance :
---
![image](https://github.com/user-attachments/assets/9a43d599-50ac-4c05-aea2-affc84dd3346)


### 9. Running

| BULAN     | PENDAPATAN ($) |
|-----------|----------------|
| April     | $12,968,820    |
| August    | $22,944,520    |
| December  | $15,349,100    |
| February  | $46,503,060    |
| January   | $19,491,780    |
| July      | $23,770,380    |
| June      | $25,003,710    |
| March     | $16,698,070    |
| May       | $11,874,870    |
| November  | $18,589,180    |
| October   | $16,261,160    |
| September | $24,273,100    |
| **Total**: | $253,727,750 |

Analisa Deskriptif Pendapatan Kategori Running :
---
| Statistik          | Nilai               |
|--------------------|---------------------|
| Mean               | 21,143,979.17       |
| Standard Error     | 2,635,864.04        |
| Median             | 19,040,480          |
| Mode               | 46,503,060          |
| Standard Deviation | 9,130,900.87        |
| Sample Variance    | 83,373,350,685,263  |
| Kurtosis           | 5.6672              |
| Skewness           | 2.1004              |
| Range              | 34,628,190          |
| Minimum            | 11,874,870          |
| Maximum            | 46,503,060          |
| Sum                | 253,727,750         |
| Count              | 12                  |

Distribusi Data Pendapatan Kategori Running :
---
![image](https://github.com/user-attachments/assets/64f14b69-5351-4c4f-a5a9-11283c3d8635)

### 10. Socks

| BULAN     | PENDAPATAN ($) |
|-----------|----------------|
| April     | $19,304,040    |
| August    | $87,860,040    |
| December  | $47,657,330    |
| February  | $53,256,730    |
| January   | $3,371,400     |
| July      | $31,853,960    |
| June      | $54,156,290    |
| March     | $25,667,810    |
| May       | $73,636,680    |
| November  | $49,328,890    |
| October   | $47,755,740    |
| September | $60,841,410    |
| **Total**: | $554,690,320 |

Analisa Deskriptif Pendapatan Kategori Socks :
---
| Statistik          | Nilai               |
|--------------------|---------------------|
| Mean               | 46,224,193.33       |
| Standard Error     | 6,750,527.26        |
| Median             | 48,542,315          |
| Mode               | 87,860,040          |
| Standard Deviation | 23,384,512.39       |
| Sample Variance    | 546,835,419,684,406 |
| Kurtosis           | 0.0456              |
| Skewness           | -0.1115             |
| Range              | 84,488,640          |
| Minimum            | 3,371,400           |
| Maximum            | 87,860,040          |
| Sum                | 554,690,320         |
| Count              | 12                  |

Distribusi Data Pendapatan Kategori Socks :
---
![image](https://github.com/user-attachments/assets/81b0328c-4b14-4173-9c8e-e9b405f22027)


### 11. Tops

| BULAN     | PENDAPATAN ($) |
|-----------|----------------|
| April     | $24,319,140    |
| August    | $47,333,720    |
| December  | $51,902,640    |
| February  | $78,054,580    |
| January   | $35,101,470    |
| July      | $34,770,090    |
| June      | $46,782,220    |
| March     | $65,583,380    |
| May       | $24,471,520    |
| November  | $17,895,210    |
| October   | $34,902,510    |
| September | $51,936,020    |
| **Total**: | $513,052,500 |

Analisa Deskriptif Pendapatan Kategori Tops :
---
| Statistik          | Nilai               |
|--------------------|---------------------|
| Mean               | 42,754,375.00       |
| Standard Error     | 5,111,278.04        |
| Median             | 40,941,845          |
| Mode               | 78,054,580          |
| Standard Deviation | 17,705,986.51       |
| Sample Variance    | 313,501,958,413,936 |
| Kurtosis           | -0.0899             |
| Skewness           | 0.5583              |
| Range              | 60,159,370          |
| Minimum            | 17,895,210          |
| Maximum            | 78,054,580          |
| Sum                | 513,052,500         |
| Count              | 12                  |

Distribusi Data Pendapatan Kategori Tops :
---
![image](https://github.com/user-attachments/assets/e2d9d5a8-7d90-4e88-bb7e-d2fcb91d6659)


### 📊 Analisis Box Plot

Tabel Kuartal
---

| Kategori     | Min        | Q1          | Q2          | Q3          | Max        |
|--------------|------------|-------------|-------------|-------------|------------|
| All          | $3,371,400 | $41,014,378 | $48,271,680 | $66,129,055 | $87,860,040 |
| Accessories  | $24,374,840| $41,014,378 | $48,271,680 | $66,129,055 | $82,041,600 |
| Bags         | $24,905,100| $35,607,140 | $48,475,710 | $62,309,765 | $79,155,950 |
| Basketball   | $5,571,940 | $15,770,963 | $19,655,270 | $29,316,495 | $47,239,280 |
| Cricket      | $7,373,020 | $23,500,913 | $29,317,615 | $38,221,190 | $79,509,210 |
| Football     | $9,394,680 | $20,252,825 | $23,026,170 | $31,594,678 | $42,133,300 |
| Lifestyle    | $4,518,700 | $17,381,300 | $28,565,360 | $32,819,398 | $50,674,230 |
| Outerwear    | $29,874,900| $50,488,230 | $63,968,310 | $70,549,848 | $86,399,680 |
| Performance  | $24,456,120| $31,531,418 | $38,414,660 | $50,009,930 | $65,196,610 |
| Running      | $11,874,870| $16,033,145 | $19,040,480 | $23,896,060 | $46,503,060 |
| Socks        | $3,371,400 | $30,307,438 | $48,542,315 | $55,827,570 | $87,860,040 |
| Tops         | $17,895,210| $32,195,448 | $40,941,845 | $51,910,985 | $78,054,580 |

Visualisasi Box Plot :
---
![image](https://github.com/user-attachments/assets/09e4c7ac-3533-40cf-a3c0-ba984e94cbeb)

Dari diagram boxplot dapat ditarik informasi sebagai berikut :

- Secara All Jenis Produk pendapatan masih bisa dibilang signifikan baik dan memiliki selisih satu sama lain cukup besar (bisa dilihat dari bentuk box yang cukup panjang).
- Jenis produk running merupakan produk dengan pendapatan paling rendah daripada jenis produk lainnya. Produk tersebut memiliki penjualan yang memusat di pendapatan rendah. Hal ini selaras dengan visualisasi diagram batang pendapatan diatas. Oleh karena itu, dapat diidentifikasi lebih lanjut mengenai strategi untuk meningkatkan jenis produk running.
- Kategori produk Footwear (Basketball, cricket, football, running, performance) memusat pada pendapatan terendah dibandingkan kategori produk lainnya.

## ✨ Kesimpulan 
Berdasarkan analisa yang telah dilakukan dapat ditarik kesimpulan sebagai berikut.

1. Trend Penjualan dan Pendapatan Produk menunjukan pola musiman yang signifikan, dengan bulan Desember sebagai puncak penjualan dan pendapatan tertinggi. Hal ini menunjukan perilaku konsumtif pada akhir tahun, yang dapat dimanfaatkan sebagai strategi untuk penjualan produk. Sebaliknya, bulan April tercatat penjualan dan pendapatan terendah sepanjang tahun. Hal ini bisa diteliti lebih lanjut sehingga menemukan strategi untuk meningkatkan angka penjualan dan pendapatan produk pada bulan tersebut.
2. Kategori Equipment mendominasi dalam hal penjualan dan pendapatan, menunjukkan bahwa produk dalam kategori ini sangat diminati oleh konsumen. Sebaliknya, kategori Footwear menunjukkan kinerja yang kurang baik meskipun memiliki variasi produk yang lebih banyak. Ini menunjukkan adanya potensi untuk meningkatkan strategi pemasaran dan pengembangan produk dalam kategori Footwear.
3. Meskipun kategori Equipment memiliki penjualan dan pendapatan tertinggi, jenis produk Outerwear dalam kategori Apparel juga menunjukkan kinerja yang sangat baik. Ini menunjukkan bahwa ada peluang untuk mengeksplorasi lebih lanjut jenis produk yang dapat meningkatkan pendapatan dalam kategori Apparel.
4. Histogram menunjukkan bahwa distribusi pendapatan tidak normal dengan skewness positif, yang berarti sebagian besar pendapatan terdistribusi pada nilai yang lebih rendah. Ini menunjukkan bahwa ada banyak produk dengan pendapatan rendah.
5. Kategori Footwear, termasuk produk seperti Basketball, Cricket, Football, Running, dan Performance, menunjukkan pendapatan yang terpusat pada nilai rendah. Ini menunjukkan bahwa ada kebutuhan untuk melakukan analisis mendalam terhadap preferensi konsumen dan potensi inovasi dalam kategori ini untuk meningkatkan penjualan.





      
      






