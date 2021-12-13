# en ubuntu con sudo apt y en debian lo hacemos con apt
  1. sudo apt update
  2. sudo apt install nginx
  # reiniciar el servicio
  1.  sudo service nginx reload --> systemctl restart nginx
  2.  sudo service nginx restart --> systemctl status nginx

# Importante
## La sintaxis del archivo de configuración tiene las siguientes características:

## Archivos de configuración de nginx
/etc/nginx/ --> se crea por defecto en la instalación de nginx
## Configuracón 
nginx.conf --> para la configuración del servicio así como para asignar los eventos y el usuario por  defecto.
## Configuramo la pagina principal
/var/www/html/index_nginx.html --> Bienvenido a mi servidor KillerZo
![img](https://github.com/abarcajoel/nginx/blob/main/img/en_navegador.PNG)
