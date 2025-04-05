FROM node:18-alpine
WORKDIR /app
COPY package.json yarn.lock ./
RUN yarn install

# Copier tout le code source
COPY . .
RUN yarn build
EXPOSE 5173
# Lancer Strapi
CMD ["yarn", "dev"]