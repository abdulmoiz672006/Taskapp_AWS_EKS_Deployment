FROM node:20-alpine3.22

WORKDIR /app

COPY package*.json ./

RUN npm install --omit=dev

COPY index.js ./
COPY db.js ./

EXPOSE 5000

CMD ["node", "index.js"]

