# afta-ssl-tls-requirement
SSL Configuration ISO-15408 and Afta lab

1.mv ssl.conf /etc/http/conf.d/ssl.conf

openssl req -x509 -newkey rsa:2048 -keyout /etc/ssl/private/apache-selfsigned.key -sha256 -nodes -days 365 -config req.cnf -out /etc/ssl/certs/apache-selfsigned.crt -extensions 'v3_req'
