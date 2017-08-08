FROM ludwigf/docker-dev


RUN dnf install -y nodejs fontconfig \
                   ruby rubygem-json ruby-devel libffi-devel && \
    gem install bundler && \
    npm install -g yarn
