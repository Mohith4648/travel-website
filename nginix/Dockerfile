FROM nginx:alpine
RUN rm -rf /usr/share/nginx/html/*
COPY ./trips-master /usr/share/nginx/html
# If you use a custom config, ensure it also listens on 80 inside
COPY ./nginix/*.conf /etc/nginx/conf.d/default.conf
EXPOSE 80 
CMD ["nginx", "-g", "daemon off;"]
