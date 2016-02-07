FROM uvatbc/ubuntu:15.10

# Keep the update separate so that Docker build system can cache it.
RUN sudo apt-get update
RUN sudo apt-get install -y \
        autoconf \
        automake \
        autopoint \
        bc \
        binutils \
        bison \
        chrpath \
        cpio \
        diffstat \
        flex \
        gawk \
        gcc-multilib \
        gettext \
        git \
        git-core \
        gperf \
        guile-2.0 \
        guile-2.0-dev \
        libasound2-dev \
        libboost-dev \
        libcurl4-openssl-dev \
        libffi-dev \
        libfontconfig1-dev \
        libglu1-mesa-dev \
        libgstreamer0.10-dev \
        libgstreamer-plugins-base0.10-dev \
        libhunspell-dev \
        libicu-dev \
        libncurses5-dev \
        libopencv-dev \
        libphonon-dev \
        libpoppler-qt4-dev \
        libqt5webkit5-dev \
        libqt5xmlpatterns5-dev \
        libsdl1.2-dev \
        libssl-dev \
        libx11-xcb-dev \
        "^libxcb.*" \
        libxcursor-dev \
        libxcomposite-dev \
        libxdamage-dev \
        libxi-dev \
        libxml2-dev \
        libxslt-dev \
        libxrandr-dev \
        libxrender-dev \
        openssl \
        qt5-default \
        qtmultimedia5-dev \
        perl \
        python \
        python-dev \
        python-django \
        python-pip \
        ruby \
        socat \
        ssh-client \
        sshpass \
        subversion \
        texi2html \
        texinfo \
        unzip \
        wget \
        xterm \
        zlib1g-dev

RUN sudo apt-get build-dep -y qt5-default

RUN sudo pip install \
        cryptography \
        mitmproxy
