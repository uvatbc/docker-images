FROM uvatbc/ubuntu:15.10

# Keep the update separate so that Docker build system can cache it.
RUN sudo apt-get update
RUN sudo apt-get install -y \
        autoconf \
        automake \
        bc \
        libssl-dev \
        libncurses5-dev \
        openssl \
        perl

