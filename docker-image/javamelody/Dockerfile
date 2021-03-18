### Dockerfile

FROM openjdk:11

COPY . /usr/src/javamelodysinglewar

CMD java -server -Dapp.home=/usr/src/javamelodysinglewar/home -Xmx128m -jar /usr/src/javamelodysinglewar/collector_server.war --httpPort=1337