FROM node:alpine

WORKDIR /app
COPY ./dist/packages/angular-client .

FROM nginx
COPY --from=0 ./app /usr/share/nginx/html