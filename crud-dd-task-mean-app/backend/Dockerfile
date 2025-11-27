# Dockerfile for backend 

FROM node:18-slim 

WORKDIR /usr/src/app

COPY backend/package*.json ./
#installing npm
RUN npm ci install --silent

#copying the backend file on to container work dir from local dir
COPY backend/ ./

# exposing the backend port
EXPOSE 3000
# executing the npm start command in container shell
CMD ["npm", "start"]