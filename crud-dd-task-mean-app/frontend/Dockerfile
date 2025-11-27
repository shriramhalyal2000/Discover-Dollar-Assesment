# dockerfile for front-end using build only
FROM node:18-alpine AS builder
# setting work dir inside the container shell
WORKDIR /App
# copying the json pacjage files for dependency installation
COPY frontend/package*.json ./

RUN npm ci

# copy the actual code files
COPY frontend/ ./
#build stage
RUN npm run build
