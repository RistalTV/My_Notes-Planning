FROM node:16.17.0-bullseye as builder

WORKDIR /app

COPY /*.json ./
COPY . .

RUN npm run build

FROM node:16.17.0-bullseye
WORKDIR /app
COPY --from=builder /app  ./
EXPOSE ${API_PORT}