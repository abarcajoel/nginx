# Crearemos un VH para los balanceos con nginx
## Configuramos los ficheros una ves instalado nginx.
1. /etc/hosts --> aquí deberemos insertar el nombre de nuestro dominio y nuestra ip.
![img](https://github.com/abarcajoel/nginx/blob/main/hosts.png)

2. /etc/nginx/ngix.conf --> debemos declarar las ip`s de nuestros servidores o nombres de dominios.
La red debe estar en el mismo dominio
.113 --> ip de servidor1
.114 --> ip de servidor2
![img](https://github.com/abarcajoel/nginx/blob/main/configuracion_http_nginx.png)

3. Comprobamos configuración
nginx -t 
Debe devolver ok

4. Reiniciamos el servicio nginx 
systemctl restart nginx


4. Comprobamos que al acceder a nuestro dominio www.joel215.org debe devolver la primera pagina de nuestro servidor1.
![img](https://github.com/abarcajoel/nginx/blob/main/primera_pagina_nginx.png)

5. Recargamos F5 y comprobamos que nos devuelve la pagina del servidor2.
![img](https://github.com/abarcajoel/nginx/blob/main/segunda_pagina_nginx.png)
