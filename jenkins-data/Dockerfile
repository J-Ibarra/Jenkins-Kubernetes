FROM debian:jessie

MAINTAINER JIbarra ibarrajj@gmail.com

# Create the jenkins user
RUN useradd -d "/var/jenkins_home" -u 1000 -m -s /bin/bash jenkins

# Create the folders and volume mount points
RUN mkdir -p /var/log/jenkins
RUN chown -R jenkins:jenkins /var/log/jenkins
VOLUME ["/var/log/jenkins", "/var/jenkins_home"]

# /var/jenkins_home/secrets/initialAdminPassword

WORKDIR /var/jenkins_home

USER jenkins