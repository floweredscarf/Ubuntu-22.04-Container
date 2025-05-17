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
        sqlite3 \
        openssh-client \
        wget \
        unzip \
        curl && \
    curl -fsSL https://deb.nodesource.com/setup_22.x -o nodesource_setup.sh && \
    bash nodesource_setup.sh && rm nodesource_setup.sh && \
    apt install -y nodejs && \
    npm install -g typescript && \
    npm install --global http-server && \
    pip3 install \
        Flask \
        Flask-session \
        fpdf \
        inflect \
        matplotlib \
        numpy \
        jupyter \
        pillow \
        pytz \
        requests && \
    echo '' >> ~/.bashrc && \
    echo '# Use bash-completion, if available' >> ~/.bashrc && \
    echo '[[ $PS1 && -f /usr/share/bash-completion/bash_completion ]] && \' >> ~/.bashrc && \
    echo '    . /usr/share/bash-completion/bash_completion' >> ~/.bashrc
