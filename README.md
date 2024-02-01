# Human Resource Analysis

Visualisasi dapat diakses melalui link berikut:
- https://public.tableau.com/views/HumanResourceDashboard_17065943141200/Dashboard3?:language=en-US&:display_count=n&:origin=viz_share_link. Pada dashboard ini User dapat memfilter data sesuai dengan status dari Attrition
- https://github.com/agungdiah/Human-Resource-Analysis/blob/master/Human%20Resource%20Dashboard.pdf

## Business Understanding
Permasalahan yang terjadi adalah masih cukup kesulitan dalam mengelola karyawan. Hal ini berimbas tingginya attrition rate (rasio jumlah karyawan yang keluar dengan total karyawan 
keseluruhan) hingga lebih dari 10%

 ## Pertanyaan Bisnis
 Apa faktor utama yang mempengaruhi attrition rate?

## Data Understanding
Dataset yang digunakan terdiri dari 34 feature atau kolom seperti
berikut.
*   EmployeeId : kolom ini berisi Id Karyawan yang bersifat unik.
*   Age : kolom ini berisi usia setiap Karyawan
*   Attrition : kolom ini berisi status pengurangan karyawan (0=tidak, 1=ya)
*   BusinessTravel : kolom ini berisi tingkat kewajiban perjalanan dalam pekerjaan (Travel_Rarely, Travel_Frequently, Non-Travel)
*   DailyRate : kolom ini memuat informasi gaji harian
*   Department : kolom ini berisi asal departemen karyawan (Research & Development, Sales, Human Resources)
*   DistanceFromHome : kolom ini berisi jarak dari tempat kerja ke rumah (dalam km)
*   Education : kolom ini berisi pendidikan karyawan 1-Below College, 2-College, 3-Bachelor, 4-Master,5-Doctor
*   EducationField : kolom ini berisi bidang pendidikan (Life Sciences,
Medical, Marketing, Technical Degree, Other, Human Resources)
*   EmployeeCount :
*   EnvironmentSatisfaction : kolom ini berisi tingkat kepuasan terhadap lingkungan (1-Low, 2-Medium, 3-High, 4-Very High)
*   Gender : kolom ini berisi gender setiap karyawan
*   Hourly Rate : kolom ini berisi informasi gaji per jam
*   JobInvolvement : kolom ini berisi gender setiap karyawan
*   JobLevel : kolom ini berisi tingkatan pekerjaan(1 to 5)
*   JobSatisfaction : kolom ini berisi tingkat kepuasan terhadap pekerjaan (1-Low, 2-Medium, 3-High, 4-Very High)
*   MaritalStatus : kolom ini berisi status pernikahan (Married, Single, Divorced)
*   MonthlyIncome : kolom ini berisi informasi gaji per bulan
*   MonthlyRate : kolom ini berisi informasi gaji pokok per bulan
*   NumCompaniesWorked : kolom ini berisi jumlah perusahaan tempat karyawan pernah bekerja selama kariernya
*   Over18 : kolom ini berisi jawaban dari pertanyaan apakah usia karyawan diatas 18
*   OverTime : kolom ini berisi jawaban dari pertanyaan apakah lembur
*   PercentSalaryHike : kolom ini berisi persentase kenaikan gaji tahun lalu
*   PerformanceRating : kolom ini berisi penilaian atau rating kinerja karyawan (1-Low, 2-Good, 3-Excellent, 4-Outstanding)
*  RelationshipSatisfaction  : kolom ini berisi tingkat kepuasan terhadap hubungan (1-Low, 2-Medium, 3-High, 4-Very High)
*  StandardHours : kolom ini berisi jumlah jam kerja standar      
*  StockOptionLevel : kolom ini berisi tingkat opsi saham yang dimiliki     
*  TotalWorkingYears : kolom ini berisi jumlah tahun kerja
*  TrainingTimesLastYear :kolom ini berisi  jumlah kali karyawan mengikuti pelatihan
*  WorkLifeBalance  : kolom ini berisi tingkat keseimbangan antara pekerjaan dan kehidupan pribadi (1-Low, 2-Good, 3-Excellent, 4-Outstanding)
*  YearsAtCompany : kolom ini berisi  jumlah tahun telah bekerja di perusahaan
*  YearsInCurrentRole : kolom ini berisi jumlah menempati jabatan
*  YearsSinceLastPromotion : kolom ini berisi tahun kenaikan jabatan terakhir kali
*  YearsWithCurrManager: kolom ini berisi jumlah tahun bekerja dengan  manajer saat ini.

## Data Preparation / Preprocessing
1. Gathering Data
2. Accessing Data
3. Cleaning Data:
   - Penanganan Missing Value
   - Penanganan Duplicated value
   - drop column yang tidak memiliki meaningful insights
   - replace those labelled numerical values with appropriate categorical values.

 ## Exploratory Data Analysis
 Visualisasi Data untuk menemukan insight:
 1.  Dari total keseluruhan karyawan proporsi karyawan yang keluar adalah 16.9% dan proporsi karyawan yang masih stay adalah 83.1%. Attrition memiliki bias yang tinggi (kecenderungan atau dominasi terhadap kategori "No")
 2.  Berdasarkan department, departemen yang paling banyak memiliki jumlah karyawan yang keluar adalah Research and Development, selanjutnya Sales Departemen  dan yang paling rendah adalah Human Resource
 3.  Berdasarkan job role, job role dengan karyawan yang jumlah keluarnya paling tinggi yaitu sebagai Laboratory Technician, sedangkan job role dengan karyawan yang jumlah keluarnya paling sedikit adalah Research Director

## Model Machine Learning
1. Pengubahan tipe data categorical menjadi numerical
2. Pemisahan Atribut dan Target
3. Resampling untuk penanganan Class Imbalance
4. Spliting data into Training and Testing
5. Model Development
- Accuracy Score of Model:  0.9602272727272727
- Precision Score of Model:  0.9597701149425287
- Recall Score of Model:  0.9597701149425287
- F1 Score of Model:  0.9597701149425287

 ## Conclusion
lima faktor utama yang mempengaruhi Attrition yaitu Overtime, MonthlyIncome, Age, DailyRate, MonthlyRate

 ## Recomendation Action
Overtime dan MonthlyIncome dua faktor utama yang berdekatan. Maka dari itu, karyawan yang lembur harus diberikan upah tambahan yang sesuai
