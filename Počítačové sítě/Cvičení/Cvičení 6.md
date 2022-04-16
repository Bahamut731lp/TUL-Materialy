# Webserver

```bash
# Instalace apache
sudo yum install httpd
service httpd start

hostname -I

# Běží na 192.168.1.52 (Adresa druhé síťovky)
student@virta0313:~$ sudo touch /var/www/html/index.html
# Změna permisí
student@virta0313:~$ sudo chmod 777 /var/www/html -R
# Vytvoření
student@virta0313:~$ hostname | grep -Eo "[0-9]+" | printf "A%s" -
# Úprava configu
student@virta0313:~$ sudo nano /etc/httpd/conf/httpd.conf


# Port forward na routeru
nano /etc/config/firewall

service firewall reload
```