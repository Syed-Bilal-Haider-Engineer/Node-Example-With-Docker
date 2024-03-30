FROM node:16

WORKDIR /usr/src/app

COPY package*.json ./
RUN --mount=type=cache,target=/root/.npm \
 npm install

COPY . .

EXPOSE 1337
CMD ["npm", "run", "dev"]