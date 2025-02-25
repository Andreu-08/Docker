# Usar la imagen base de PHP 7.4 con FastCGI Process Manager
FROM php:7.4-fpm

# Actualizar los repositorios e instalar las extensiones necesarias para PDO MySQL
RUN apt-get update && apt-get install -y \
    && docker-php-ext-install pdo pdo_mysql

# Consejos y trucos:
# - Usa 'docker build -t nombre_imagen .' para construir la imagen.
# - Usa 'docker run nombre_imagen' para ejecutar el contenedor.
# - Verifica los logs del contenedor con 'docker logs id_contenedor' para solucionar problemas.
# - Usa 'docker exec -it id_contenedor /bin/bash' para acceder al contenedor en ejecución y depurar.
