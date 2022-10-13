FROM node:16

WORKDIR /front-app

COPY . .

RUN npm i
RUN npm run build

RUN mkdir -p /var/www/html
RUN mv build/* /var/www/html

RUN rm -f /front-app