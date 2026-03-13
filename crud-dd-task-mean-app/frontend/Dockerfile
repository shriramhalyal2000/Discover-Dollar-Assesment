# frontend Dockerfile

FROM node:18-alpine

WORKDIR /app

COPY ./package*.json ./
RUN npm install

COPY . .

# edited package.jason to include host 0.0.0.0 and port 4200 when it starts
EXPOSE 4200

CMD ["npm", "start"]
