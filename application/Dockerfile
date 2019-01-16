FROM node:slim

RUN apt-get -y update

RUN mkdir -p /usr/src/app

WORKDIR /usr/src/app

COPY package.json ./

RUN npm install

COPY . .

# If you are building your code for production
# RUN npm install --only=production

EXPOSE 3000

CMD [ "npm", "start" ]