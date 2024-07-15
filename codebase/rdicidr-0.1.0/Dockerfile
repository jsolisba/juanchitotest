FROM node:15 as builder

# Establece el directorio de trabajo dentro del contenedor
WORKDIR /app

# Copia el archivo package.json y package-lock.json
COPY package*.json ./

# Instala las dependencias del proyecto
RUN npm install

# Copia el resto del código de la aplicación
COPY . .

# Exponer el puerto en el que tu aplicación estará corriendo
EXPOSE 3000

# Comando para ejecutar la aplicación
CMD ["npm", "start"]
