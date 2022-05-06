ARG DEBIAN_FRONTEND=noninteractive
FROM jenkins/ssh-agent:4.2.1-jdk11
USER root 
RUN apt-get update && apt-getinstall-y curl git python python-pip3
RUN groupadd -g 997 docker \
&& usermod -aG docker jenkins \
&& curl -fsSL https://get.docker.com/ | sh