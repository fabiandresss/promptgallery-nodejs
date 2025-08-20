FROM node:18-alpine

WORKDIR /app

# Copiar package.json primero (para cache de Docker)
COPY package*.json ./

# Instalar dependencias
RUN npm install

# Copiar código fuente
COPY . .

# Exponer puerto 4000
EXPOSE 4000

# Comando por defecto
CMD ["npm", "run", "dev"] 
