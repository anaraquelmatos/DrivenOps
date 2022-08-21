FROM node:16

WORKDIR /usr/src

COPY . .

RUN npm i && npm run build

RUN mkdir -p /var/www/html

RUN mv build/* /var/www/html

WORKDIR /

RUN rm -rf /usr/src