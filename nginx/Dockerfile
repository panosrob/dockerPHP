FROM nginx:latest

ADD ./nginx.conf /etc/nginx/
RUN rm /etc/nginx/conf.d/default.conf && \
    mkdir /etc/nginx/sites-available/
COPY ./sites/*.conf /etc/nginx/sites-available/
