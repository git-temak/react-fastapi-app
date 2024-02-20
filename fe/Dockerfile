FROM node:20-alpine

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install

COPY . .

EXPOSE 3000

ENV REACT_APP_API_URL='http://localhost:8000' \
    REACT_APP_LESSON_DAY='day1'

CMD ["npm", "run", "start"]