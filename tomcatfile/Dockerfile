FROM daocloud.io/library/java:openjdk-8-jre-alpine
MAINTAINER caojin <1257063655@qq.com>
COPY ./apache-tomcat-8.5.42.tar.gz /usr/local/
RUN cd /usr/local/ && tar xf apache-tomcat-8.5.42.tar.gz
RUN cd /usr/local/apache-tomcat-8.5.42/webapps/ && rm -rf ROOT
COPY ./ROOT.war /usr/local/apache-tomcat-8.5.42/webapps/
ENTRYPOINT ["/usr/local/apache-tomcat-8.5.42/bin/catalina.sh","run"]
