FROM uvatbc/ubuntu:15.10

# Keep the update separate so that Docker build system can cache it.
RUN sudo apt-get update
RUN sudo apt-get install -y \
        autoconf \
        automake \
        bc \
        libncurses5-dev \
        libssl-dev \
        openssl \
        perl

