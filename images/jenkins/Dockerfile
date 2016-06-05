FROM jenkins:latest
# See more about Jenkins + Docker outside Docker
# http://container-solutions.com/running-docker-in-jenkins-in-docker

USER root
# Install Docker binary.
ENV DOCKER_VERSION 1.9.1
RUN wget -nv https://get.docker.com/builds/Linux/x86_64/docker-$DOCKER_VERSION -O /usr/bin/docker && \
      chmod +x /usr/bin/docker

# Add user jenkins to "sudo" group.
RUN apt-get update \
      && apt-get install -y sudo \
      && rm -rf /var/lib/apt/lists/*
RUN echo "jenkins ALL=NOPASSWD: ALL" >> /etc/sudoers

USER jenkins
# Install additional Jenkins plugins.
COPY plugins.txt /usr/share/jenkins/plugins.txt
RUN /usr/local/bin/plugins.sh /usr/share/jenkins/plugins.txt
