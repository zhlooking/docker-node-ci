FROM node:10.21.0-alpine3.11

LABEL maintainer="zhang hao <zhlookin@gmail.com>"

RUN echo Asia/Shanghai > /etc/timezone \
  && sed -i 's/dl-cdn.alpinelinux.org/mirrors.tuna.tsinghua.edu.cn/g' /etc/apk/repositories \
  && apk add --no-cache openssh-client rsync git \
  && yarn config set registry 'https://registry.npm.taobao.org'

# yarn global add eslint & eslint-config-zcool  to skip `yarn install` in lint stage
