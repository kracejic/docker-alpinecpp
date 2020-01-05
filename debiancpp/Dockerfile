FROM debian:testing


# install dependencies and clean up
RUN apt-get update -y && \
    apt-get upgrade -y && \
    apt-get install -y make gcc cmake git clang-tidy vim bash cppcheck && \
    apt-get clean && \
    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*

RUN git clone https://github.com/kracejic/dotfiles-minimal.git ~/bin && cd ~/bin && ./install.sh

CMD ["bash"]
