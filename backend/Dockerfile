# Imagen base
FROM node:20

# Carpeta de trabajo
WORKDIR /app

# Copiar archivos
COPY package*.json ./
RUN npm install

# Copiar el resto del código
COPY . .

# Exponer el puerto
EXPOSE 5000

# Comando para arrancar
CMD ["npm", "run", "dev"]
