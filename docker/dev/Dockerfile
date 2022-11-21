FROM alpine:3.17

WORKDIR /home/node/app

# Node.js
RUN apk add --update nodejs npm
RUN apk add --update npm

# Ruby
RUN apk update
RUN apk add ruby-dev
RUN apk update && apk add --no-cache build-base

# npm install
RUN npm install --global npm@^7

# Grunt
RUN npm install --global grunt-cli

# Sass
RUN gem install sass