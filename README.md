# Big-Data
Nama : Abdul Aziz
Nim : 312210022
Kelas C3


# DISINI SAYA MENGGUNAKAN wsl di windows untuk mengakses linux ubuntu
![image](https://github.com/user-attachments/assets/dfac93f2-2a2c-468e-8fda-f7b0df80ea0d)

Langkah Pertama 
# 1. Persiapan Folder Proyek dan Struktur
Jalankan perintah berikut di terminal WSL untuk membuat struktur folder:
        # Buat folder proyek
        mkdir mqtt_project && cd mqtt_project

        # Buat subfolder
        mkdir mqtt_server sensor_service db

        # Masuk ke masing-masing folder untuk buat file
        touch mqtt_server/mosquitto.conf
        touch mqtt_server/Dockerfile
        touch sensor_service/Dockerfile
        touch sensor_service/sensor_publisher.py
        touch db/init.sql
        touch docker-compose.yml .env
# 2. Konfigurasi Mosquitto (MQTT Broker)

- <h3>1</h3>
Masuk ke ke mqtt_server/mosquitto.conf dengan cara ketik "nano mqtt_server/mosquitto.conf"
dan isi dengan perintah berikut                                                                 
   ![image](https://github.com/user-attachments/assets/c4851d51-f81a-4789-bff7-46a66eb61f70)

- <h3>2</h3>
Lalu masuk ke mqtt_server/Dockerfile.
dengan mengetikan nano mqtt_server/Dockerfile
dan isi seperti berikut.
  ![image](https://github.com/user-attachments/assets/55e7ee4b-7c84-422e-a5b0-aebe3297d1cd)

- <h3>3</h3> lalu masuk ke nano sensor_service/Docekerfile dan isi sebagai berikut
  
![image](https://github.com/user-attachments/assets/6cd59a8c-a3a1-4e1b-b4f4-6357ce93ef4c)

- <h3>4</h3>
lalu masuk ke nano sensor_service/sensor_publisher.py dan masukan isinya seperti berikut
![image](https://github.com/user-attachments/assets/25960d37-f5e5-411c-b0b7-6f7aa9a25158)

- <h3>4</h3> Kemudian buat Dockerfile untuk sensor_service:
isi seperti berikut 
![image](https://github.com/user-attachments/assets/1d6dd425-1f78-4ae7-8f99-8f254dd70193)

- <h3>5 MySQL Database Setup </h3>

Edit file db/init.sql untuk membuat tabel yang akan menyimpan data sensor:
![image](https://github.com/user-attachments/assets/88702e0f-b99f-4da7-81ef-0c1e5dde5b38)

- <h3>6 Docker Compose </h3>
Edit file docker-compose.yml untuk mendefinisikan layanan-layanan Docker:
![image](https://github.com/user-attachments/assets/685187a5-6b6b-4fd5-98c2-a04ba9a4b567)

- <h3> docker compose </h3>
![image](https://github.com/user-attachments/assets/1c6ffd17-ebb9-4e5b-aad6-7350bd6485f1)


- <h3> File .env (Opsional) </h3>
dengan masuk nano .env
Untuk menjaga keamanan data, kita dapat menyimpan variabel environment di file .env. Contohnya:
![image](https://github.com/user-attachments/assets/aeea9e45-175f-4a98-b3be-82a55409e4a2)











