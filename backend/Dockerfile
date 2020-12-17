FROM node:14-alpine

# Create working directory
RUN mkdir -p /app/backend
WORKDIR /app/backend

COPY package.json /app/backend
COPY yarn.lock /app/backend

RUN yarn install

COPY . /app/backend

CMD ["yarn", "start"]
