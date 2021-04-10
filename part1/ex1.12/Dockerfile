FROM node:14.16

EXPOSE 5000

WORKDIR /usr/src/app

COPY . .
RUN node -v && npm -v && npm i && npm run build && npm install -g serve

CMD serve -s -l 5000 build