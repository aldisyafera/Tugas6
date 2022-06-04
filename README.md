# Tugas6

Nama : Aldi Syafera

Kelas : TI.20.D.1

NIM : 312010008

matkul : Sistem Basis Data

.Masuk ke databse nama_nim

![image](https://user-images.githubusercontent.com/103243638/172019437-5cef0eb7-6000-4237-bf34-8658e5bce575.png)

. Lakukan proses backup dan recovery dengan sql dari database tugas seblumnya !

backup

![image](https://user-images.githubusercontent.com/103243638/172019501-308d8266-f489-4d3f-a95d-1e83d1e0f51b.png)

Jika proses backup berhasil maka akan muncul file backuppada direktori C:\xampp\mysql\data\nama database

![image](https://user-images.githubusercontent.com/103243638/172019537-7ff09436-ca82-430b-b4da-406be3615487.png)

Recovery

Data yang telah di-backup dapat dikembalikan kapan saja bila diperlukan. Sintaks SQL yang digunakan adalah LOAD DATA INFILE. Perintah yang dijalankan adalah

LOAD DATA INFILE ‘Nama_backup_file’ INTO TABLE nama_table ;

![image](https://user-images.githubusercontent.com/103243638/172019605-7351d022-1f03-4fc0-a811-7cf5fa2cc074.png)

![image](https://user-images.githubusercontent.com/103243638/172019660-e9bb6d23-0a14-4f7a-ad7f-87d26f4653f6.png)

![image](https://user-images.githubusercontent.com/103243638/172019711-76c64d01-c2b3-40b6-9120-8e919ad8848e.png)

. Lakukan proses backup dan recovery dengan sqldump dari database tugas seblumnya !

![image](https://user-images.githubusercontent.com/103243638/172019828-4af81fd0-3f08-40a8-ae14-82b4072be955.png)

![image](https://user-images.githubusercontent.com/103243638/172019872-b4a24ef4-fa43-40ea-8707-4f34fcb56011.png)

Tulisakan script cron job untuk melakukan backup otomatis setiap hari minggu jam 12 malam !

crontab –e

00**7myqldump -u root -p aldi_312010008>aldi_312010001_backup.sql
