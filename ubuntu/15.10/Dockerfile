FROM ubuntu:15.10

RUN apt-get update && \
    apt-get -y dist-upgrade && \
    apt-get install -y \
        bash-completion \
        build-essential \
        vim \
        sudo

RUN echo ". /etc/bash_completion" >> /root/.bashrc

CMD /bin/bash

RUN useradd -ms /bin/bash admin && \
    echo "admin:admin" | chpasswd && \
    adduser admin sudo && \
    echo "admin ALL=(ALL) NOPASSWD:ALL" >> /etc/sudoers

USER admin
ENV HOME /user/admin
WORKDIR /user/admin

RUN sudo chown -R admin:admin /user/admin
RUN echo ". /etc/bash_completion" >> /user/admin/.bashrc && \
    echo "alias ls='ls --color' ; alias ll='ls -l'" >> /user/admin/.bashrc
