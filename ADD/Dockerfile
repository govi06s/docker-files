FROM almalinux:9
RUN dnf install nginx -y && \
    rm -rf usr/share/nginx/html/index.html
ADD https://github.com/daws-81s/expense-infra-dev/blob/main/readme.MD usr/share/nginx/html/index.html
RUN chmod +x usr/share/nginx/html/index.html
ADD sample-1.tar /tmp
CMD ["nginx", "-g", "daemon off;"]
