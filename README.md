# afta-ssl-tls-requirement
SSL Configuration based on ISO-15408 and web protection profile Afta labs
instance on apache on redhat OS


```sh
mv ssl.conf /etc/http/conf.d/ssl.conf
```

```sh
openssl req -x509 -newkey rsa:2048 -keyout /etc/ssl/private/apache-selfsigned.key -sha256 -nodes -days 365 -config req.cnf -out /etc/ssl/certs/apache-selfsigned.crt -extensions 'v3_req'
```
