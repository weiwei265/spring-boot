FROM frolvlad/alpine-oraclejdk8:slim
VOLUME /tmp
ADD msfw-user.jar msfw-user.jar
CMD java -Xmx512m -Xms256m -Djava.security.egd=file:/dev/./urandom -jar /msfw-user.jar
EXPOSE 9081
ENV TZ=Asia/Shanghai
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone  