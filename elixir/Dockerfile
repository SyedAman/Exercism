FROM elixir:1.6.4-alpine

# Download and install Exercism CLI
RUN wget https://github.com/exercism/cli/releases/download/v2.4.1/exercism-linux-64bit.tgz; \
    tar -xzvf exercism-linux-64bit.tgz; \
    mkdir ~/bin; \
    mv exercism ~/bin/; \
    export PATH=$HOME/bin:$PATH; \
    echo 'export PATH=$HOME/bin:$PATH' >> ~/.bashrc

# ENTRYPOINT bash

# Create working directory
WORKDIR /root/exercism/elixir
VOLUME /root/exercism/elixir

ENTRYPOINT ~/bin/exercism fetch elixir && sh
