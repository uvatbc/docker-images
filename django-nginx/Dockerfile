FROM uvatbc/ubuntu:15.10

# Keep the update separate so that Docker build system can cache it.
RUN sudo apt-get update
RUN sudo apt-get -y install \
        build-essential \
        git \
        nginx \
        python-dev \
        python-django \
        python-pip \
        python-setuptools \
        python-software-properties \
        sqlite3 \
        ssh-client \
        sshpass \
        supervisor

RUN sudo pip install --upgrade \
        django \
        uwsgi
