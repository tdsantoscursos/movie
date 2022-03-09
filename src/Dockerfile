FROM node:lts-alpine@sha256:2c6c59cf4d34d4f937ddfcf33bab9d8bbad8658d1b9de7b97622566a52167f2b
ENV NODE_ENV production
WORKDIR /usr/src/app
COPY --chown=node:node . /usr/src/app
RUN npm ci --only=production
USER node
EXPOSE 8181
CMD ["node", "server.js"]