FROM node:8

WORKDIR /app

ADD package-lock.json .
ADD package.json .
ADD yarn.lock .
RUN yarn install
ADD . .
RUN npm run build

ENTRYPOINT ["npm"]
CMD ["run","service"]



