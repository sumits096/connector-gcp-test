FROM node:14

WORKDIR /usr/src/app

COPY ./connector/package*.json ./

RUN npm install

COPY . .

RUN npm run build

CMD [ "npm", "run", "node dist/main.js" ]
