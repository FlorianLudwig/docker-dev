FROM fedora:26

ENV HOME /tmp/home

RUN dnf -y install dnf-plugins-core && \
    dnf config-manager \
        --add-repo \
        https://download.docker.com/linux/fedora/docker-ce.repo && \
    dnf install -y docker-ce \
                   gcc gcc-c++ redhat-rpm-config make \
                   git patch findutils \
                   bzip2 xz \
                   zlib-devel \
                   which \
                   xorg-x11-server-Xvfb xorg-x11-xauth \
                   rsync && \
    ln -s /bin/python3 /bin/python && \
    ln -s /bin/pip3 /bin/pip && \
    pip install cookiecutter && \
    mkdir /tmp/home
