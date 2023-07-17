# **Business Problem Understanding**

**Context**

Perusahaan travel asuransi adalah perusahaan yang menyediakan layanan asuransi perjalanan kepada pelanggan. Mereka menawarkan berbagai jenis polis asuransi yang mencakup perlindungan terhadap kerugian atau risiko yang terkait dengan perjalanan seperti pembatalan perjalanan, keterlambatan penerbangan, kehilangan bagasi, atau kecelakaan selama perjalanan. Salah satu tantangan yang dihadapi oleh perusahaan adalah mengelola klaim asuransi dengan baik dan meminimalkan penyalahgunaan klaim yang tidak sah. 
Ketika seorang pelanggan mengajukan klaim, perusahaan harus melakukan pengecekan dan verifikasi yang memakan waktu dan sumber daya. Jika klaim tidak valid atau disengaja, perusahaan harus menanggung kerugian finansial dan reputasi yang dapat berdampak negatif pada bisnis mereka.

**Target :**

No : Tidak mengajukan klaim asuransi

Yes : Mengajukan klaim asuransi

**Problem Statement**

Perusahaan travel asuransi menghadapi tantangan dalam mengelola klaim asuransi dengan baik dan meminimalkan penyalahgunaan klaim yang tidak sah. Proses pengecekan dan verifikasi klaim yang memakan waktu dan sumber daya dapat mengakibatkan kerugian finansial dan reputasi yang merugikan perusahaan. Selain itu, ada risiko kesalahan dalam memprediksi pelanggan yang benar-benar mengajukan klaim, yang dapat mengakibatkan pelanggan yang berhak mendapatkan klaim tidak mendapatkannya.

**Goals**

Perusahaan travel insurance memiliki keinginan untuk memiliki kemampuan dalam memprediksi apakah calon pemegang polis akan mengajukan klaim atau tidak. Hal ini bertujuan untuk menghindari kerugian finansial bagi perusahaan dengan memastikan bahwa calon pemegang polis yang dipilih kemungkinan besar tidak akan mengajukan klaim.

**Analytic Approach**

- Mengumpulkan Data: Mengumpulkan informasi klaim asuransi yang relevan.
- Menyusun Data: Membersihkan dan mengatur data agar mudah dianalisis.
- Mengembangkan Informasi: Menemukan pola dan informasi penting dari data yang ada.
- Memilih Pendekatan: Memilih metode yang tepat untuk memprediksi perilaku klaim.
- Melatih Model: Melatih model menggunakan data yang telah disiapkan.
- Menilai Kinerja: Mengevaluasi sejauh mana model dapat mengidentifikasi klaim dengan benar.
- Mengoptimalkan Model: Mengubah model agar lebih baik dalam mengenali klaim yang benar.

**Metric Evaluation**

Type 1 Error (False Positive) 

Model memprediksi bahwa seorang pelanggan akan mengajukan klaim (Claim = Yes), padahal sebenarnya pelanggan tersebut tidak mengajukan klaim (Claim = No)

Type 2 Error (False Negative)

Model memprediksi bahwa seorang pelanggan tidak akan mengajukan klaim (Claim = No), padahal pelanggan tersebut sebenarnya mengajukan klaim (Claim = Yes)

Dengan memilih F2 Score sebagai metric evaluasi, perusahaan akan dapat menilai sejauh mana model mereka efektif dalam mengenali pelanggan yang benar-benar mengajukan klaim asuransi dengan lebih fokus pada recall. Tujuan utama adalah meminimalkan false negatives (Type 2 Error) agar sebanyak mungkin pelanggan yang berhak mendapatkan klaim dapat terdeteksi dengan benar.
