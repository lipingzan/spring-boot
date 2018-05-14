#FROM java:8
FROM frolvlad/alpine-oraclejdk8:slim
VOLUME /tmp
ADD spring-boot-1.0.0.jar app.jar
#RUN bash -c 'touch /app.jar'
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]

#RUN sh -c 'touch /app.jar'
#ENV JAVA_OPTS=""
#ENTRYPOINT [ "sh", "-c", "java $JAVA_OPTS -Djava.security.egd=file:/dev/./urandom -jar /app.jar" ]
# docker run -e JAVA_OPTS='-Xms128m -Xmx256m -Dspring.profiles.active=test' -it pumelo/test-1.0.0 /bin/bash
# docker run -d --name springboot01 -p 8080:8080 -e JAVA_OPTS='-Xms128m -Xmx256m -Dspring.profiles.active=test' harbor.lipingzan.cn/test/spring-boot:0.0.1