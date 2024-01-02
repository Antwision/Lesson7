FROM ubuntu:22.04
RUN apt update && apt install \
    git \
    default-jdk \
    maven -y \
    &&  rm -rf /var/lib/apt/lists/*
RUN mkdir -p /usr/src/app7/
WORKDIR /usr/src/app7/
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git
WORKDIR /usr/src/app7/boxfuse-sample-java-war-hello/
RUN mvn package
# RUN cp ./target/hello-1.0.war $CATALINA_HOME/webapps
