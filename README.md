## Install Exercism CLI

### Ubuntu
Install the tar from GitHub. Extract. Add to path.

```sh
$ wget https://github.com/exercism/cli/releases/download/v2.4.1/exercism-linux-64bit.tgz && tar -xzvf exercism-linux-64bit.tgz && mkdir ~/bin && mv exercism ~/bin/ && export PATH=$HOME/bin:$PATH && echo 'export PATH=$HOME/bin:$PATH' >> ~/.bashrc && exercism --version
```
