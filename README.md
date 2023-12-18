## _OS SERVER & SISTEMA ADMIN_

## 22.83.0866_Muhamad Akbar Baihaqqy Ramadhani

## Service yang diinstall di iso centos 7:

- apache2
- SSH
- winscp

## installasi apache2

perbarui sistem
```
sudo yum update
```
install apache2
```
sudo yum install httpd

```
setting
```
sudo systemctl start httpd
sudo systemctl enable httpd
```
tambahkan rule firewall
```

sudo firewall-cmd --permanent --add-service=http
sudo firewall-cmd --reload
```
test website
```
http://192.168.56.105
````
![image](https://github.com/Paksel/FINAL-SERVER/assets/145017392/57812a58-2785-4698-bef5-f8294e544b0f)

## installasi openssh

perbarui sistem
```
sudo yum update
```
install openssh
```
sudo yum install openssh-server
```
start dan enable layanan ssh
```
sudo systemctl start sshd
sudo systemctl enable sshd
```
konfigurasi firewall
```
sudo firewall-cmd --permanent --add-service=ssh
sudo firewall-cmd --reload
```
uji koneksi ssh
```
ssh root@192.168.56.105
```
![image](https://github.com/Paksel/FINAL-SERVER/assets/145017392/5d5ac4d1-f348-45c2-8b5b-1f32dcd9b777)

##  winscp
```
https://winscp.net/eng/index.php untuk memindahkan file ke iso yang digunakan.
````
Masukkan nama user, ip, port, dan juga password untuk bisa mengakses winscp agar bisa memindahkan file 
![image](https://github.com/Paksel/FINAL-SERVER/assets/145017392/74d2fb46-48f3-493d-9458-5b48c352a412)
