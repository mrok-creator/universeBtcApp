FROM node:18.16.0
WORKDIR /usr/src/app
COPY package*.json ./
RUN npm install
COPY . .
RUN npm run build service-app
EXPOSE 8080
CMD ["node","dist/apps/service-app/main"]