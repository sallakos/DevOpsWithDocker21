FROM node:14.16

EXPOSE 5000

WORKDIR /usr/src/app

COPY . .
RUN node -v && npm -v && npm i && npm install -g serve

ENV REACT_APP_BACKEND_URL="http://localhost:8080"

RUN npm run build

CMD serve -s -l 5000 build