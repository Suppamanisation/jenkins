FROM ubuntu:16.04

RUN apt-get -y update && apt-get install -y \ 
	nginx
RUN apt-get clean && rm -rf /var/lib/apt/lists/*

RUN echo "daemon off;" >> /etc/nginx/nginx.conf

COPY . /var/www/

CMD ["nginx"]

EXPOSE 80
