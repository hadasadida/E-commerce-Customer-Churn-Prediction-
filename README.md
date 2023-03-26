# E-commerce Customer Churn Prediction-

dataset : https://www.kaggle.com/datasets/ankitverma2010/ecommerce-customer-churn-analysis-and-prediction

Created by :
1. Jasmine Alya Nisa
2. Ichsan Kurnia S
3. Hada Sadida
4. Bima Dwica Ananto
5. Wisnu Nirwono
6. Nita Dwi Indahsari
7. Laurensius Rio Wiratama
8. Steven Zalukhu

(This project is reupload and revised from original source (https://github.com/Rocket3FPRakamin/Rocket-3-FP))

_________________________________________________________________________________________________________________________________________________________________________

## Stage 0 (Preparation)
### Problem Statement (Menentukan problem yang akan diselesaikan dengan model dari dataset)
Terdapat tingkat churn yang cukup tinggi pada data yang dimiliki yaitu 16.8%. Sehingga perusahaan ingin mengurangi tingkat churn dengan memberikan penawaran promo kepada customer yang terindikasi churn.
### Goal (Menentukan tujuan utama yang ingin dicapai)
Mengatasi customer yang akan churn, dengan mengetahui faktor apa saja yang mempengaruhi customer churn.
### Objective (Menentukan sasaran akhir yang dicapai dari tujuan yang telah ditentukan)
1) Membuat model untuk memprediksi customer yang berpotensi churn. 
2) Memberi rekomendasi promo bagi customer yang terindikasi akan churn.
### Business Metric (Mengukur ketercapaian objective yang telah ditentukan)
Customer churn rate.

## Stage 1 
### Data Exploration
a) Attribute :
1) CustomerID										(Unique customer ID)
2) Tenure												(Tenure of customer in organization)
3) PreferredLoginDevice					(Preferred login device of customer)
4) CityTier											(City tier)
5) WarehouseToHome							(Distance in between warehouse to home of customer)
6) PreferredPaymentMode					(Preferred payment method of customer)
7) Gender												(Gender of customer)
8) HourSpendOnApp								(Number of hours spend on mobile application or website)
9) NumberOfDeviceRegistered			(Total number of deceives is registered on particular customer)
10) PreferedOrderCat						(Preferred order category of customer in last month)
11) SatisfactionScore						(Satisfactory score of customer on service)
12) MaritalStatus								(Marital status of customer)
13) NumberOfAddress							(Total number of added added on particular customer)
14) Complain										(Any complaint has been raised in last month)
15) OrderAmountHikeFromlastYear	(Percentage increases in order from last year)
16) CouponUsed									(Total number of coupon has been used in last month)
17) OrderCount									(Total number of orders has been places in last month)
18) DaySinceLastOrder						(Day Since last order by customer)
19) CashbackAmount							(Average cashback in last month)

b) Target :
Churn														(Churn flag)

### EDA (Exploratory Data Analysis)
1) Univariate dan Multivariate Analysis pada masing-masing fitur/atribut terhadap target
2) Business insight 

## Stage 2
### Data Cleansing 
1) Handling missing value
2) Handling outlier 
3) Feature transformation
4) Feature encoding
5) Handle class imbalance 

### Feature Engineering
Semua fitur digunakan untuk modelling

## Stage 3
### Modeling 
Tedapat 6 model yang dibuat yaitu:
1) Decision tree
2) Logistic regression
3) K-nearest neighbor 
4) ADABoost
5) XGBoost
6) Random Forest 

### Evaluation 
Dari 6 model yang telah dibuat dipilih model XGBoost dengan pertimbangan nilai ROC-AUC yang paling sesuai.

## Conclusion
Berdasarkan model yang telah dibuat terdapat 2 feature importance teratas yaitu Tenure dan Complain. Berdasarkan 2 feature importance teratas tersebut dapat disimpulkan bahwa 2 faktor teratas customer melakukan churn yaitu Tenure dan Complain. Untuk mengatasi faktor tersebut dapat dilakukan penanganan terhadap customer baru yang akan melakukan churn tersebut. 

a. Tenure 

1) Pada Tenure 0-2 bulan pertama customer lebih banyak melakukan churn. Hal ini dapat diasumsikan bahwa customer dengan Tenure 0-2 bulan pertama merupakan customer baru dari e-commerce. Sehingga dapat diatasi dengan memberikan package promo cashback untuk mencegah potensi churn terhadap customer baru. 

2) Selain itu dapat memberi pesan notifikasi secara rutin bagi customer yang sudah pernah memesan untuk dapat kembali memesan produk-produk lainnya (repeat order).

3) Kemudian dapat memberikan reward berupa membership ataupun voucher-voucher berskala dengan seberapa aktif/loyal customer tersebut.

b. Complain

1) Customer yang melakukan complain lebih banyak melakukan churn dibanding dengan yang tidak. Hal ini dapat diasumsikan bahwa customer service dari e-commerce terhadap customer tidak memuaskan. Sehingga dapat menyediakan pelayanan 24/7 yang sigap (dapat difilter melalui AI terlebih dahulu atau langsung kontak customer service).

2) Untuk customer complain, dapat dibuatkan channel khusus untuk feedback, sekaligus memberikan voucher yang adaptif terhadap kerugian yang dialami.

3) Memberikan garansi jaminan produk sebagai cara preventif mencegah/meminimalisir adanya customer complain.











