# Step 1: Use Nginx base image
FROM nginx:alpine

# Step 2: Copy your website content
# This copies the actual website files from your 'trips-master' folder
COPY ./trips-master /usr/share/nginx/html

# Step 3: Copy the config using a wildcard (*)
# This will find your file whether it's named 'ngnix.conf', 'nginx.conf', or 'default.conf'
# as long as it is inside the 'nginix' folder.
COPY ./nginix/*.conf /etc/nginx/conf.d/default.conf

# Step 4: Expose port and start
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
