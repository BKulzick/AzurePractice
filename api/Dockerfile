FROM gradle:4.2.1-jdk8-alpine
VOLUME /opt
#VOLUME /tmp
#COPY . /home/gradle/project
#WORKDIR /home/gradle/project
#USER root
#RUN chmod -R 777 /home/gradle/project
#USER gradle

#RUN ./gradlew clean build --stacktrace
#USER root

#COPY ./build/libs/retroquest.jar app.jar
#RUN chmod -R 777 app.jar
WORKDIR /opt
CMD env GRADLE_USER_HOME=/opt/gradlehome ./gradlew clean build && java -jar build/libs/retroquest.jar
