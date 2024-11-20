FROM node:20.10-buster-slim

WORKDIR /home/node/
USER node
COPY . .

RUN npm install --production

ENTRYPOINT ["node", "/lib/main.js"]
HEALTHCHECK CMD curl --fail http://localhost:3000 || exit 1
