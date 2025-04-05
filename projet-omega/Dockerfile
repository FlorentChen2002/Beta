FROM node:18

# Définir le dossier de travail
WORKDIR /srv/app

# Copier les fichiers nécessaires
COPY package.json yarn.lock ./

# Installer les dépendances
RUN yarn install

# Copier tout le code source
COPY . .

EXPOSE 1337
# Lancer Strapi
CMD ["yarn", "develop"]