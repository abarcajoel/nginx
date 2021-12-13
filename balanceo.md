# Crearemos un VH para los balanceos con nginx
## Configuramos los ficheros una ves instalado nginx.
1. /etc/hosts --> aquí deberemos insertar el nombre de nuestro dominio y nuestra ip.
![img](https://github.com/abarcajoel/nginx/blob/main/hosts.png)

2. /etc/nginx/ngix.conf --> debemos declarar las ip`s de nuestros servidores o nombres de dominios.
![img](https://github.com/abarcajoel/nginx/blob/main/configuracion_http_nginx.png)

3. Comprobamos configuración
nginx -t 
![img]()

4. Reiniciamos el servicio nginx 
systemctl restart nginx
![img]()

4. Comprobamos que al acceder a nuestro dominio www.joel215.org debe devolver la primera pagina de nuestro servidor1.
![img]()

5. Recargamos F5 y comprobamos que nos devuelve la pagina del servidor2.
![img]()
