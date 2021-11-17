# Author: https://github.com/hrodic/
#
# Build instruction
# -------------------------------------
# docker build -t context-mapper:6.6.0 .

FROM openjdk:8-slim
WORKDIR /usr/src/myapp

RUN apt-get update && apt-get install -y wget graphviz

RUN wget https://repo1.maven.org/maven2/org/contextmapper/context-mapper-cli/6.6.0/context-mapper-cli-6.6.0.tar && \
    tar xvf context-mapper-cli-6.6.0.tar

ENTRYPOINT [ "./context-mapper-cli-6.6.0/bin/cm" ]
