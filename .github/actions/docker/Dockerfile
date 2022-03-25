FROM node:16-alpine

COPY ./dist .

RUN npm install --production

ENTRYPOINT ["node", "index.js"]