# Dockerfile for React client

# Build react client
FROM node:18.20.2-alpine

# Working directory be app
WORKDIR /app

COPY package*.json ./

###  Installing dependencies

RUN npm install --force --loglevel verbose

# copy local files to app folder
COPY . .

EXPOSE 3000

CMD ["npm","start"]