FROM nginx:alpine
COPY . /usr/share/nginx/html
EXPOSE 80
RUN chown -R nginx:nginx /var/cache/nginx /etc/nginx/
USER nginx

CMD ["nginx", "-g", "daemon off;"]