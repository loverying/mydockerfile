FROM nginx:1.14-alpine
MAINTAINER caojin <1257063655@qq.com>
COPY ./nginx.conf /etc/nginx/nginx.conf
RUN mkdir -p /opt/wwwroot
ADD myapp.zip /opt/wwwroot/
RUN cd /opt/wwwroot/ && unzip myapp.zip
CMD /bin/sh -c 'nginx -g "daemon off;"'
