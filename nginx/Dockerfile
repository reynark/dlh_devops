FROM ubuntu:18.04
LABEL maintainer=adursun
RUN apt-get update && apt-get install -y nginx && apt-get clean && echo "daemon off;" >> /etc/nginx/nginx.conf
EXPOSE 80
ENTRYPOINT ["nginx"] ## CMD da olur ama ENTRYPOINT daha saglam olur
