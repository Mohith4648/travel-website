# Use the small, fast Alpine Nginx image
FROM nginx:alpine

# Step 1: Remove any default Nginx website files
RUN rm -rf /usr/share/nginx/html/*

# Step 2: Copy your travel project files
# We use the dot (.) to copy the CONTENTS of trips-master
COPY ./trips-master /usr/share/nginx/html

# Step 3: Skip custom config for now to ensure the site loads
# Nginx will automatically use its internal default config on port 80

EXPOSE 80

CMD ["nginx", "-g", "daemon off;"]
