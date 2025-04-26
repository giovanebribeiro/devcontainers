FROM mcr.microsoft.com/devcontainers/base:alpine-3.20 AS dev

RUN rm /bin/sh && ln -s /bin/bash /bin/sh

RUN id -u vscode &> /dev/null || useradd -ms /bin/bash vscode
RUN mkdir -p /home/vscode/.ssh
RUN chown -R vscode:vscode /home/vscode/.ssh

CMD [ "sleep", "infinity" ]