# Usar la imagen base de Node.js versión 14 en Alpine Linux
FROM node:14-alpine

# Establecer el directorio de trabajo dentro del contenedor
WORKDIR /app

# Copiar los archivos package.json y package-lock.json al directorio de trabajo
COPY app/package*.json ./

# Instalar las dependencias definidas en package.json
RUN npm install

# Copiar el resto de los archivos de la aplicación al directorio de trabajo
COPY app/ .

# Exponer el puerto 3000 para acceder a la aplicación
EXPOSE 3000

# Comando para iniciar la aplicación Node.js
CMD ["npm", "start"]

# Consejos y trucos:
# - Usa 'docker build -t nombre_imagen .' para construir la imagen.
# - Usa 'docker run -p 3000:3000 nombre_imagen' para ejecutar el contenedor y mapear el puerto 3000 del host al contenedor.
# - Verifica los logs del contenedor con 'docker logs id_contenedor' para solucionar problemas.
# - Usa 'docker exec -it id_contenedor /bin/sh' para acceder al contenedor en ejecución y depurar.
