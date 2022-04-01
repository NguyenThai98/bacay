FROM hk86/centos:jdk8
# https://github.com/SergeyZh/docker-centos6-java/blob/master/jdk8/Dockerfile
ENV TZ=Asia/Ho_Chi_Minh
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
# Adding cacerts file from current Java disto to "conf" directory of Tomcat

ADD . /var/www/

WORKDIR /var/www/

RUN chmod +x main