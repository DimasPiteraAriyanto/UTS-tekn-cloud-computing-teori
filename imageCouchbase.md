2. Memilih Image yang menarik, pull, dan menjalankannya.

Saya memilih image dari official image milik couchbase
![couchbase](https://github.com/XabaraNeanthal/UTS-tekn-cloud-computing-teori/blob/master/gambar-02.png)

Untuk menarik image tersebut maka dapat dilakukan cara sebagai berikut :

a. Docker pull couchbase
![pull](https://github.com/XabaraNeanthal/UTS-tekn-cloud-computing-teori/blob/master/gambar-03.png)
b. Run Couchbase Server docker container 
docker run -d --name db -p 8091-8094:8091-8094 -p 11210:11210 couchbase
![container](https://github.com/XabaraNeanthal/UTS-tekn-cloud-computing-teori/blob/master/gambar-04.png)
c. Selanjutnya, kunjungi http://localhost:8091 host untuk melihat Web Console untuk memulai pengaturan Couchbase Server.
![index1](https://github.com/XabaraNeanthal/UTS-tekn-cloud-computing-teori/blob/master/gambar-05.png)
![setup](https://github.com/XabaraNeanthal/UTS-tekn-cloud-computing-teori/blob/master/gambar-06.png)
Dapat dilakukan configurasi sendiri atau mengikuti default yang ada.
![configur](https://github.com/XabaraNeanthal/UTS-tekn-cloud-computing-teori/blob/master/gambar-07.png)
d. Setelah dapat dijalankan dan digunakan dapat dimatikan dengan cara menggunakan perintah docker container rm --force db
![rm](https://github.com/XabaraNeanthal/UTS-tekn-cloud-computing-teori/blob/master/gambar-08.png)