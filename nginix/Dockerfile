# Step 1: Use Nginx base image
FROM nginx:alpine

# Step 2: Copy your website content
# We go up one level (..) because Dockerfile is inside 'nginix' 
# and the HTML files are in 'trips-master'
COPY ./trips-master /usr/share/nginx/html

# Step 3: Copy your custom config file
# Your file is named ngnix.conf
COPY ./nginix/ngnix.conf /etc/nginx/conf.d/default.conf

# Step 4: Expose port and start
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
