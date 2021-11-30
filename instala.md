# en ubuntu con sudo apt y en debian lo hacemos con apt
  1. sudo apt update
  2. sudo apt install nginx
  # reiniciar el servicio
  1.  sudo service nginx reload --> systemctl restart nginx
  2.  sudo service nginx restart --> systemctl status nginx

# importante
## La sintaxis del archivo de configuración tiene las siguientes características:

Ajustes: todos los ajustes se inician con los respectivos nombres de las variables. Los argumentos se conectan o separan por medio de espacios y siempre van acompañados de un punto y coma al final.
worker_connections 768;
Ajustes genéricos: algunos ajustes, como la variable events, incluyen argumentos que, a su vez, representan ajustes con sus propios argumentos. Estas subdirectivas se enmarcan con llaves ({}).
# events {  worker_connections 768;  multi_accept on;}
Amohadilla (#): las directivas (instrucciones) que están deshabilitadas son precedidas por una almohadilla. Cuando se elimina la marca, se activa la configuración correspondiente del servidor. Por ejemplo, en el caso de
# multi_accept on;
la opción para aceptar varios clientes al mismo tiempo está desactivada.

Saltos de línea y espacios múltiples: nginx interpreta los saltos de línea y múltiples espacios como un único espacio. Al configurar nginx, es posible aprovechar esta ventaja y velar por una estructura clara y legible del archivo de configuración. 
 Para acceder a más información acerca de los módulos individuales, así como a otros tutoriales para la configuración de servidores proxy basados en un servidor nginx, puedes visitar la documentación oficial en su página web.