FROM node:slim

WORKDIR /web-app
ADD package.json /web-app/
RUN npm install
ADD . /web-app

CMD ["node", "app.js"]
