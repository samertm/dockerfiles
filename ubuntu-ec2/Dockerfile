FROM ubuntu:14.04

COPY sudoers-ubuntu-init /etc/sudoers.d/sudoers-ubuntu-init
RUN chmod 440 /etc/sudoers.d/sudoers-ubuntu-init

RUN adduser --home /home/ubuntu --shel /bin/bash --disabled-password --gecos 'Ubuntu' ubuntu

RUN mkdir /home/ubuntu/.ssh
RUN chown ubuntu:ubuntu /home/ubuntu/.ssh
RUN chmod 700 /home/ubuntu/.ssh

USER ubuntu
