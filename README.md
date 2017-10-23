# Nginx
```
sudo yum install epel-release

sudo yum install nginx

sudo systemctl start nginx

sudo systemctl enable nginx

sudo firewall-cmd --permanent --zone=public --add-service=http

sudo firewall-cmd --permanent --zone=public --add-service=https
```
### Allow port redirecting
```
sudo firewall-cmd --permanent --zone=public --add-masquerade

sudo firewall-cmd --permanent --zone=public --add-forward-port=port80:proto=tcp:toport=8080

sudo firewall-cmd --permament --zone=public --add-forward-port=port443:proto=tcp:toport8080

sudo firewall-cmd --reload
```
