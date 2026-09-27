FROM ubuntu:26.04
LABEL maintainer="partha09"

ENV DEBIAN_FRONTEND=noninteractive

RUN apt-get update && \
    apt-get dist-upgrade -y && \
    apt-get install -y --no-install-recommends \
        # Build tools
        cmake \
        build-essential \
        extra-cmake-modules \
        gettext \
        git \
        curl \
        # Qt5 build deps
        libqt5x11extras5-dev \
        qtdeclarative5-dev \
        qt3d5-dev \
        # KF5 build deps
        libkf5config-dev \
        libkf5coreaddons-dev \
        libkf5guiaddons-dev \
        libkf5configwidgets-dev \
        libkf5windowsystem-dev \
        libkf5iconthemes-dev \
        libkf5kcmutils-dev \
        libkf5style-dev \
        kirigami2-dev \
        # Qt6 build deps
        qt6-base-dev \
        qt6-declarative-dev \
        # KF6 build deps
        libkf6coreaddons-dev \
        libkf6colorscheme-dev \
        libkf6config-dev \
        libkf6guiaddons-dev \
        libkf6i18n-dev \
        libkf6iconthemes-dev \
        libkf6windowsystem-dev \
        libkf6kcmutils-dev \
        libkf6style-dev \
        libkirigami-dev \
        # Window decorations (KDecoration3)
        libkdecorations3-dev \
    && apt-get clean \
    && rm -rf /var/lib/apt/lists/*
