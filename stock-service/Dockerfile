FROM node:18

WORKDIR /app

COPY package*.json ./

RUN npm install

RUN apt-get update && apt-get install -y netcat-openbsd

COPY . .

RUN npm install -g prisma

CMD ["npm", "run", "dev"]







