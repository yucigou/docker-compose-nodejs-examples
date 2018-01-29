FROM node:8.9.4

RUN mkdir /src

RUN npm install express-generator -g

WORKDIR /src
COPY app /src/app

ADD app/package.json /src/package.json
RUN npm install

EXPOSE 3000

CMD node app/bin/www