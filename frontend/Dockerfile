#DOCKERFILE FRONTEND
FROM node:14-alpine

WORKDIR /app

# on ajoute '/app/node_modules/.bin' to $PATH
ENV PATH /app/node_modules/.bin:$PATH

# on installe les dépendances de l'appli
COPY package*.json ./


RUN npm install


# Copie les fichier de l'app
COPY . .

EXPOSE 3000
CMD ["npm", "start"]