FROM node:lts-alpine@sha256:2c6c59cf4d34d4f937ddfcf33bab9d8bbad8658d1b9de7b97622566a52167f2b
WORKDIR /app
COPY ./package*.json ./
RUN npm install
COPY . .
EXPOSE 8181
CMD ["node", "./server.js"]