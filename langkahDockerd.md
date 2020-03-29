Langkah-langkah :

a. Docker pull couchbase, digunakan untuk mengambil image yang ada pada official docker tersebut sehingga dapat digunakan pada local. Setelah melakukan perintah pull yang sesuai dengan yang ada pada perintah image official tersebut maka akan terdownload semua source yang dibutuhkan untuk menjalankan image tersebut, kecepatan dalam mengambil source tersebut tergantung kecepatan internet milik user. Terdapat banyak image yang ada di explore dockerhub dan pilih saja yang dibutuhkan atau yang ingin dipelajari.
![pull](https://github.com/XabaraNeanthal/UTS-tekn-cloud-computing-teori/blob/master/gambar-03.png)
b. Run Couchbase Server docker container menggunkana perintah **docker run -d --name db -p 8091-8094:8091-8094 -p 11210:11210 couchbase**. **Docker run** yang digunakan untuk setiap image berbeda sesuai dengan settingan yang ada pada image tersebut, kebetulan docker run yang digunakan pada couchbase sudah tercantum pada image officialnya sehingga hanya perlu mengcopy bagian tersebut untuk menjalankan containernya.
![container](https://github.com/XabaraNeanthal/UTS-tekn-cloud-computing-teori/blob/master/gambar-04.png)
c. Selanjutnya, kunjungi **http://localhost:8091** host untuk melihat Web Console untuk memulai pengaturan Couchbase Server.
![index1](https://github.com/XabaraNeanthal/UTS-tekn-cloud-computing-teori/blob/master/gambar-05.png)
![setup](https://github.com/XabaraNeanthal/UTS-tekn-cloud-computing-teori/blob/master/gambar-06.png)
Dapat dilakukan configurasi sendiri atau mengikuti default yang ada.
![configur](https://github.com/XabaraNeanthal/UTS-tekn-cloud-computing-teori/blob/master/gambar-07.png)
d. Setelah dapat dijalankan dan digunakan dapat dimatikan dengan cara menggunakan perintah **docker container rm --force db**, db digunakan untuk mematikan container database. Untuk menggunakan container yang lain saat sudah selesai digunakan dapat menggunakan perintah **docker container rm --force** atau selebihnya dapat dilihat di [docker rm](https://docs.docker.com/engine/reference/commandline/rm/)
![rm](https://github.com/XabaraNeanthal/UTS-tekn-cloud-computing-teori/blob/master/gambar-08.png)