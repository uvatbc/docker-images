FROM uvatbc/qt4

# Keep the update separate so that Docker build system can cache it.
RUN sudo apt-get update
RUN sudo apt-get install -y \
        libcurl4-openssl-dev \
        libboost-dev \
        libhunspell-dev \
        libopencv-dev \
        libpoppler-qt4-dev

