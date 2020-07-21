FROM debian:testing


# install dependencies and clean up
RUN apt-get update -y && \
    apt-get install -y make gcc g++ cmake git clang-tidy bash python3 gcovr  && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

RUN update-alternatives --install /usr/bin/python python /usr/bin/python3 1 && update-alternatives  --set python /usr/bin/python3

RUN git clone https://github.com/kracejic/dotfiles-minimal.git ~/bin && cd ~/bin && ./install.sh

CMD ["bash"]
