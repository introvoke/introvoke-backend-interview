FROM node:14-alpine

# See the docker-compose.ymp file for the port that is set
ARG EXPOSE_PORT

WORKDIR /server

ENV PATH /node_modules/.bin:$PATH
COPY package.json ./
COPY package-lock.json ./
RUN npm install --silent
EXPOSE $EXPOSE_PORT
COPY . .

CMD ["npm", "start"]
