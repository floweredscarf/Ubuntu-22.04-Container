FROM ubuntu:22.04
RUN apt update && \
    apt install --no-install-recommends --yes \
        clang \
        make \
        python3 \
        python3-pip \
        python3-venv \
        openjdk-21-jdk \
        bash-completion \
        git \
        nodejs \
        npm \
        sqlite3 \
        openssh-client && \
    npm install --global http-server && \
    pip3 install \
        cs50 \
        flask \
        flask-session \
        jupyter \
        pillow \
        pytz \
        requests && \
    echo '' >> ~/.bashrc && \
    echo '# Use bash-completion, if available' >> ~/.bashrc && \
    echo '[[ $PS1 && -f /usr/share/bash-completion/bash_completion ]] && \' >> ~/.bashrc && \
    echo '    . /usr/share/bash-completion/bash_completion' >> ~/.bashrc
