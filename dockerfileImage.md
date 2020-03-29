Membuat DockerFile

1. Membuat dockerfile dengan aplikasi editor yang dapat digunakan.
![vscode](https://github.com/XabaraNeanthal/UTS-tekn-cloud-computing-teori/blob/master/gambar-09.png)
2. Pada baris pertama yaitu perintah yang digunakan untuk memanggil base image milik ubuntu yang nanti akan didownload secara otomatis saat menjalankan dockerfile, lalu pada baris 2 menggunakan output CMD untuk menampilkan keluarannya.
3. Setelah selesai membuat dockerfile dapat dilakukan build image melalui docker quickstart terminal jika menggunkan docker toolbox atau git jika menggunakan docker desktop lalu shorthand -t yang dimana berguna seperti membuat container dilanjutkan dengan nama image dan tagnya, dan setelah selesai build dapat dilakukan cek apakah sudah terbuild atau belum menggunakan perintah "docker images ls". 
![image](https://github.com/XabaraNeanthal/UTS-tekn-cloud-computing-teori/blob/master/gambar-11.png)
Pada gambar diatas masih tertulis tag namenya 1.0 akan tetapi yang digunakan adalah tag name 2.0 seperti dibawah ini 
![image](https://github.com/XabaraNeanthal/UTS-tekn-cloud-computing-teori/blob/master/gambar-18.png)

Untuk mengecek isi dari image yang sudah terbuild dapat menggunakan perintah **docker run**
![image](https://github.com/XabaraNeanthal/UTS-tekn-cloud-computing-teori/blob/master/gambar-10.png)
4. Setelah sudah dicek ada dan dapat berjalan seta mengeluarkan output yang diharapkan maka dapat langsung melakukan push ke repo yang ada di dockerhub dengan cara menggunkan perintah **docker push dimas99/myimage:tagname** karena sebelumnya sudah membuat repo **myimage** terlebih dahulu maka dapat menggunakan perintah tersebut. tagname berisi tag yang ada
Tetapi sebelumnya dilakukan commit didocker karena harus mendownload image yang telah dibuat menjadi lokal dan membuat nama dan tag baru untuk image lokalnya. 
![image](https://github.com/XabaraNeanthal/UTS-tekn-cloud-computing-teori/blob/master/gambar-14.png)
Untuk melakukan commit harus ada container terlebih dahulu. Cara mengeceknya dengan cara mengetikan perintah **docker ps**
![image](https://github.com/XabaraNeanthal/UTS-tekn-cloud-computing-teori/blob/master/gambar-16.png)

Jika belum memiliki container maka dapat membuatnya terlebih dahulu dengan cara yang ada di web [Create Container](https://docs.docker.com/engine/reference/commandline/create/)
![image](https://github.com/XabaraNeanthal/UTS-tekn-cloud-computing-teori/blob/master/gambar-17.png)

5. Hasil push dapat dilihat di sini [dokcerhub](https://hub.docker.com/repository/docker/dimas99/utstcc175610079)
![image](https://github.com/XabaraNeanthal/UTS-tekn-cloud-computing-teori/blob/master/gambar-15.png)

gambar 12 dan 13 kesalahan dalam melakukan push