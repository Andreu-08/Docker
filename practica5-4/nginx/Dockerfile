# Usar la imagen base de Nginx en su última versión
FROM nginx:latest

# Copiar el archivo de configuración de Nginx al directorio de configuración
COPY ./default.conf /etc/nginx/conf.d/default.conf

# Consejos y trucos:
# - Usa 'docker build -t nombre_imagen .' para construir la imagen.
# - Usa 'docker run -p 80:80 nombre_imagen' para ejecutar el contenedor y mapear el puerto 80 del host al contenedor.
# - Verifica los logs del contenedor con 'docker logs id_contenedor' para solucionar problemas.
# - Usa 'docker exec -it id_contenedor /bin/bash' para acceder al contenedor en ejecución y depurar.
