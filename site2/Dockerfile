# Dockerfile for site2
FROM node:16

WORKDIR /app

COPY package.json ./
COPY package-lock.json ./
RUN npm install

COPY . .

RUN npm run build

EXPOSE 5174
CMD ["npm", "run", "preview"]
