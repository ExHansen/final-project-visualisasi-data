  # Final Project: Visualisasi Data

Transforming raw data into impactful visual stories using Looker Studio dan Google Colab.

![Screenshot 2025-06-16 195013](https://github.com/user-attachments/assets/1f0c3a34-df44-41a8-ac5b-e706da02a376)

Link Looker Studio: https://lookerstudio.google.com/reporting/badb667f-6afb-407e-b7df-1bb0520279fd

Link PPT: https://drive.google.com/file/d/1AlYfE8wklnyLvKAEi52vePLqQOm8U7HP/view?usp=sharing

Link Proses Explarotary Data Analysis (EDA): https://colab.research.google.com/drive/1g-cmfIxypNeCfSeGDGeiEojTKAP8FLqX#scrollTo=cdadacd7

Link Proses Preprocessing: https://colab.research.google.com/drive/1bEwbO8WYoHNsFmPKtwjTOaeOwKtxwfNw#scrollTo=99747a75

## Overview
`final-project-visualisasi-data` empowers developers to analyze, process, and visualize data effectively. This project provides essential tools for **data exploration** and **visualization**.

### Why Use final-project-visualisasi-data?
- 📊 **Exploratory Data Analysis (EDA):** Identify patterns and anomalies effortlessly.
- 🛠 **Data Preprocessing:** Clean and structure raw data for accuracy.
- 🌍 **User-Friendly Interface:** Designed for both technical and non-technical users.
- 🔄 **Dynamic Interaction:** Enables iterative exploration before deeper analysis.
- 🔑 **Data Integrity:** Ensures reliable insights for modeling.

Dalam Proses Preprocessing dan EDA terlihat bahwa:
- Semua data dilakukan penghilangan whitespace/spasi ganda
- tgl_lahir diubah Dtypenya dari object ke datetime dan menambahkan kolom umur
- tahun_sertifikasi karena ada nilai 0 didalam tahun sertifikasi tetapi terdapat sertifikasi, maka akan diubah menjadi 1 sebagai tulisan bahwa: 1 = Memiliki sertifikasi, tidak ada tahun 0 = Tidak ada sertifikasi, tidak ada tahun
- tgl_jabatan_akademik ubah Dtypenya dari object ke datetime
- fakultas Terdapat kesalahan untuk Hubungan Internasional yang seharusnya FISIP, tetapi dalam data tertulis FH, Manajemen seharusnya berada di FEB, tetapi di data tertulis berada di FISIP, Sains Biomedis seharusnya berada di FK, tetapi berada di FIKES
- rumpun_ilmu, pangkat, jabatan_akademik, sertifikasi isi null agar Looker studio dapat memparsing datanya tanpa error
- id_pegawai, jk, stat_aktif, stat_pegawai, ikatan_kerja, pendidikan, jenj_prodi, prodi datanya sudah baik

Selain itu, dalam Dashboard dapat dilihat, bahwa:
Pegawai aktif Kampus XYZ didominasi dosen tetap berpendidikan S2 dengan rata-rata usia 44,2 tahun. Namun, masih terdapat tantangan seperti rendahnya proporsi dosen bersertifikasi, minimnya jumlah pegawai S3, ketimpangan distribusi jabatan akademik, dan kekurangan SDM pada beberapa rumpun ilmu, yang perlu ditindaklanjuti untuk peningkatan mutu dan keberlanjutan institusi.
