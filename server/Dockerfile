FROM node:18.20.2-alpine
WORKDIR /app
COPY package*.json ./
RUN npm config set strict-ssl false && npm ci --only=production
COPY . .
EXPOSE 8080
CMD ["node", "index.js"]