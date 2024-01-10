FROM ubuntu:22.04
RUN apt update && apt install \
    git \
    maven -y \
    &&  rm -rf /var/lib/apt/lists/*
WORKDIR /usr/src/app/
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git
WORKDIR /usr/src/app/boxfuse-sample-java-war-hello/
RUN mvn package