FROM node

WORKDIR /app/my-app

COPY package*.json ./

RUN npm install

COPY . .
RUN chown -R node /app/my-app/node_modules

USER node

EXPOSE 3000

CMD ["npm", "start"]