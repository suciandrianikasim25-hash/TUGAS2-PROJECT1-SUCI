# TUGAS2-PROJECT1-SUCI
# LANGKAH 1
# Membuat Direktori untuk 3 Departemen marketinng engineering hr beserta subfoldernya
(https://drive.google.com/file/d/19qBAuNQVcPNU87_zW2Tv7oOBQaIEIX1G/view?usp=sharing)
~~~
#lubuntu@suci:~ mkdir -p marketing/documents marketing/archives
~~~
~~~
#lubuntu@suci:~ mkdir -p engineering/documents engineering/archives
~~~
~~~
#lubuntu@suci:~ mkdir -p hr/documents hr/archives
~~~

# Membuat subfolder di masing-masing direktori
https://drive.google.com/file/d/1mtEC0HPjUca88aHkfY_kyQseYYsPReZR/view?usp=sharing

~~~
#lubuntu@suci:~cd marketing
#lubuntu@suci:~cd documents
#lubuntu@suci:~cd documents
#lubuntu@suci:~cd documents
#lubuntu@suci:~touch m_laporan.docx.docx
#lubuntu@suci:~touch m_arsip.pdf
#lubuntu@suci:~cd ..
#lubuntu@suci:~cd engineering
#lubuntu@suci:~cd documents
#lubuntu@suci:~touch e_laporan.docx
#lubuntu@suci:~cd ..
#lubuntu@suci:~cd archives
#lubuntu@suci:~touch e_arsip.pdf
#lubuntu@suci:~cd ..
#lubuntu@suci:~cd hr
#lubuntu@suci:~cd documents
#lubuntu@suci:~touch h_laporan.docx
#lubuntu@suci:~cd ..
#lubuntu@suci:~cd archives
#lubuntu@suci:~touch h_arsip.pdf
~~~

# LANGKAH 2
# Memindahkan file yang salah tempat ke direktori yang benar
https://drive.google.com/file/d/1hmor0EXH1_YKH7kBzuxio6brAvgv2UCZ/view?usp=sharing GAMBAR

~~~
mv images/file11.jpg marketing/documents
~~~
~~~
mv images/file11.jpg Marketing/documents
~~~
~~~
mv images/file11.jpg Marketing/documents
~~~
# Membuat backup di folder archives
https://drive.google.com/file/d/1i5aFQQcO1QE6JC_NhCigzCXjLwV5MfP3/view?usp=sharing

~~~
cp -r marketing/Dokuments/marketing.docx marketing/Archives
~~~
~~~
cp -r engineering/documents/engineering.docx engineering/archives
~~~
~~~
cp -r hr/documents/hr.docx hr/archives
~~~

# LANGKAH 3
# Permision/membatasi hak akses di setiap folder
https://drive.google.com/file/d/1i5aFQQcO1QE6JC_NhCigzCXjLwV5MfP3/view?usp=sharing

~~~
sudo groupadd Marketing
~~~
~~~
sudo groupadd Enginering
~~~
~~~
sudo groupadd HR 
~~~

# Mengubah kepemilikan folder dan semua isi di dalamnya
https://drive.google.com/file/d/12p8vOVvhKgBVD3_lyX4dn81PqPwszwqB/view?usp=sharing

~~~
sudo chgrp -r marketinng marketing
~~~
~~~
sudo chgrp -rengineering engineering
~~~
~~~
sudo chgrp -r hr hr
~~~

# Mengatur izin permision folder
https://drive.google.com/file/d/1o26I52KIE1WVA7SwpvU04REx0c3ffd9q/view?usp=sharing

~~~
sudo chmod 770 Marketing
~~~
~~~
sudo chmod 770 Engineering
~~~
~~~
sudo chmod 770 HR
~~~

# LANGKAH 4
# Menampilkan file pdf -7 hari yang lalu
https://drive.google.com/file/d/1xrygBkUhrezeDyXsIKSdfHlNaI0uCGlN/view?usp=sharing

~~~
find . -type f -name "*.pdf" -mtime -7
~~~
