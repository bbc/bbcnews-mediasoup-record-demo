FROM node:14

WORKDIR /home/node/app

COPY . .

RUN npm install --also=dev

RUN npm run build

CMD [ "npm", "run", "dev" ]

