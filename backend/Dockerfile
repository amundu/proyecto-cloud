# creamos una variable
ARG PORT=4200
# traemos la imagen de node 12 con kernel de alpine
FROM node:12-alpine
# label para agregar metadatos
LABEL autor="Alexis"
# cremos el directorio de la app
WORKDIR /usr/src/app
# copiamos el archivo a nuestra carpeta 
COPY package*.json ./
# instalamos las dependencias
RUN npm install
# copiamos todo al directorio de trabajo
COPY . .
# exponemos el puero
EXPOSE ${PORT}
# corremos el comando para nuestra app
CMD [ "npm", "start" ]