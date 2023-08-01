
FROM nginx:stable-alpine

RUN addgroup --gid 1000 mygroup
RUN adduser --system --no-create-home --disabled-password --disabled-login --uid 1000 --ingroup mygroup myuser
COPY . /usr/share/nginx/html
WORKDIR /var/www/html

RUN chown -R myuser:mygroup .

USER myuser
