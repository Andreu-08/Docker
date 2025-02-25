# Usar la imagen base de Alpine Linux, una distribución ligera
FROM alpine

# Actualizar los repositorios e instalar Apache y PHP
RUN apk update && apk add apache2 php7-apache2 php7

# Crear un usuario sin privilegios para ejecutar el servidor web
RUN adduser -D -g  www-data www-data

# Cambiar la propiedad del directorio web al usuario creado
RUN chown -R www-data:www-data /var/www/localhost/htdocs/

# Copiar el archivo index.php al directorio web
COPY index.php /var/www/localhost/htdocs/index.php

# Exponer el puerto 80 para acceder al servidor web
EXPOSE 80

# Comando para iniciar Apache en primer plano
CMD ["/usr/sbin/httpd", "-D", "FOREGROUND"]

# Consejos y trucos:
# - Usa 'docker build -t nombre_imagen .' para construir la imagen.
# - Usa 'docker run -p 80:80 nombre_imagen' para ejecutar el contenedor y mapear el puerto 80 del host al contenedor.
# - Verifica los logs del contenedor con 'docker logs id_contenedor' para solucionar problemas.
# - Usa 'docker exec -it id_contenedor /bin/sh' para acceder al contenedor en ejecución y depurar.







