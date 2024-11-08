FROM node:18-alpine

WORKDIR /app

COPY package*.json ./
RUN rm -rf node_modules
RUN rm package-lock.json
RUN npm install

COPY . .

RUN npm run build

EXPOSE 3000

RUN npm install -g serve
CMD ["serve", "-s", "build", "-l", "3000"]
