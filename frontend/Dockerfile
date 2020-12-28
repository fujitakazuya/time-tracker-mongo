FROM node:14.15.3-alpine3.12

WORKDIR /var/www/html

COPY ./time-tracker ./time-tracker

WORKDIR /var/www/html/time-tracker
RUN apk add --update-cache vips-dev
RUN yarn install && yarn build

CMD ["yarn", "start"]
