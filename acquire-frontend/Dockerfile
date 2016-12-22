FROM nginx:1.10-alpine
RUN apk add --no-cache nodejs git python make g++
RUN npm install webpack -g
WORKDIR /usr/share/nginx/html
RUN git clone https://github.com/svera/acquire-frontend.git
ADD config.js acquire-frontend/frontend/config.js
RUN cd acquire-frontend && npm install && npm run build
RUN rm /etc/nginx/conf.d/default.conf
ADD nginx.conf /etc/nginx/nginx.conf
