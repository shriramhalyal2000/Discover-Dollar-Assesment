# Dockerfile for backend 

FROM node:18-slim 

WORKDIR /usr/src/app

COPY ./package*.json ./
#installing npm
RUN npm install --silent

#copying the backend file on to container work dir from local dir
COPY ./ ./
ENV PORT=8080
# exposing the backend port
EXPOSE 8080
# executing the npm start command in container shell
CMD ["npm", "start"]