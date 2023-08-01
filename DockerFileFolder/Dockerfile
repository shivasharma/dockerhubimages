FROM nginx:alpine
COPY . /usr/share/nginx/html
EXPOSE 80
RUN chown -R nginx:nginx /var/cache/nginx /etc/nginx/
RUN useradd -m nginx && echo "nginx:nginx" | chpasswd && adduser nginx sudo
USER nginx

CMD ["nginx", "-g", "daemon off;"]