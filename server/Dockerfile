FROM node:16.17.0-bullseye

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install

COPY . .

# COPY --from=server /usr/src/app/dist ./dist

CMD ["node", "dist/main"]