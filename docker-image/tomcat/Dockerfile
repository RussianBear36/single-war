### Dockerfile

FROM tomcat:9-jdk11

#Removing default applications like manager
ENV DEPLOY_DIR $CATALINA_HOME/webapps/
RUN rm -rf $DEPLOY_DIR/*

#Preparing default app home folder
RUN mkdir $CATALINA_HOME/work/singlewar-home

#Setting environment variables
ENV spring.profiles.active=docker
ENV JAVA_OPTS="-Dapp.home=$CATALINA_HOME/work/singlewar-home"

#Deploying applications to tomcat
COPY app.war $DEPLOY_DIR