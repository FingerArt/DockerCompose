FROM nginx:1.12

WORKDIR /usr/share/nginx/html

#copy配置
COPY default.conf /etc/nginx/conf.d/

#源码
ADD https://github.com/FingerArt/DockerCompose.git .
