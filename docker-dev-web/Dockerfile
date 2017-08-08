FROM ludwigf/docker-dev

RUN dnf install -y nodejs fontconfig \
                   ruby rubygem-json ruby-devel libffi-devel && \
    gem install bundler && \ # the version in dnf is too old
    npm install -g yarn
