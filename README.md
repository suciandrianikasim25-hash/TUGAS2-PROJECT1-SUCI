# TUGAS2-PROJECT1-SUCI
# LANGKAH 1
# Membuat Direktori untuk 3 Departemen marketinng engineering hr  beserta subfoldernya
GAMBAR
~~~
#lubuntu@suci:~ mkdir -p marketing/documents marketing/archives
~~~
~~~
#lubuntu@suci:~ mkdir -p engineering/documents engineering/archives
~~~
~~~
#lubuntu@suci:~ mkdir -p hr/documents hr/archives
~~~
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
# Memindahkan file yang salah tempat ke direktori
yang benar
# GAMBAR

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
# GAMBAR
~~~
cp -r marketing/Dokuments/marketing.docx marketing/Archives
~~~
~~~
cp -r engineering/documents/engineering.docx engineering/archives
~~~
~~~
cp -r hr/documents/hr.docx hr/archives
~~~

# Menampilkan isi folder marketing engineering hr
# GAMBAR

~~~
tree
~~~

# LANGKAH 3
# Permision/membatasi hak akses di setiap folder
# GAMBAR

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
# GAMBAR

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

~~~
sudo chmod 770 Marketing
~~~
~~~
sudo chmod 770 Engineering
~~~
~~~
sudo chmod 770 HR
~~~

# LATIHAN 4
# Menampilkan file pdf -7 hari yang lalu
# DEFINISI GAMBAR

~~~
find . -type f -name "*.pdf" -mtime -7
~~~
