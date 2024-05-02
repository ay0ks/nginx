## nginx
-----
```bash
sudo su
cd /etc
git clone https://github.com/ay0ks/nginx.git
cd nginx
mkdir certs.d # This is where you should put certificates and keys
mkdir logs.d # This is where logs will appear 
```
```bash
systemctl restart nginx
```
