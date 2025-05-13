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

