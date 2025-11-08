FROM node:22

WORKDIR /app

COPY package*.json .

# Install dependencies(clean install)
RUN npm ci 

COPY src/index.js index.js

EXPOSE 3000

CMD [ "node", "index.js" ]