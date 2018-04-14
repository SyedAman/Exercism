FROM elixir

# Download and install Exercism CLI
RUN wget https://github.com/exercism/cli/releases/download/v2.4.1/exercism-linux-64bit.tgz
RUN tar -xzvf exercism-linux-64bit.tgz
RUN mkdir ~/bin
RUN mv exercism ~/bin/
RUN export PATH=$HOME/bin:$PATH
RUN echo 'export PATH=$HOME/bin:$PATH' >> ~/.bashrc

# ENTRYPOINT bash

# Create working directory
WORKDIR /app
VOLUME /app

ENTRYPOINT ~/bin/exercism fetch elixir && bash
