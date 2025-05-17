# docker-cloud
Repo untuk mendalami docker di cloud menggunakan laynanan EC2 AWS dengan OS Ubuntu
# Launch instance Ubuntu di EC2
- Masuk ke AWS Console
- Cari service EC2
- Pilih OS Ubuntu
# Instalasi Docker di Ubuntu
- Masuk ke terminal Ubuntu menggunakan Command Prompt
- sudo apt-get update
- sudo apt install docker.io
- sudo systemctl start docker
- sudo systemctl enable docker
- sudo docker --version
# Instalasi Web Server nginx
- docker pull nginx
- docker run --name docker-nginx -p 80:80 nginx
- sudo docker ps-a
- Masuk ke browser melalui IP Publik yang didapat dari EC2, lalu halaman nginx akan tampil
# Perintah Dasar Docker
- docker pull nginx:latest (berfungsi untuk mengunduh dokcer image dari registrasi Dockerhub)
- docker container create nginx (berfungsi untuk membuat container dari suatu image)
- docker start web-server-1 (berfungsi untuk menjalankan container)
- docker ps (berfungsi untuk melihat container yang berjalan)
- docker ps -a (berfungsi untuk melihat semua container yang ada)
- docker stop web-server-1 (berfungsi untuk menghentikan container)
- docker rm web-server-1 (berfungsi untuk menghapus container)
- docker images (berfungsi untuk melihat daftar images yang ada)
- docker rmi nginx:latest (berfungsi untuk menghapus image yang ada)
- docker run --name [nama-container] -d -p [port local]:[port container] [nama image]:[tag]
  - contoh penulisan perintah: docker run --name reach-app -d -p 8080:80 reach-basic:latest (berfungsi untuk mengambil docker image, membuat, dan menjalankan containernya)
