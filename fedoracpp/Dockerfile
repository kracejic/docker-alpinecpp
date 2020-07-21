FROM fedora:latest

# Set the working directory to /app
# WORKDIR /app

# Copy the current directory contents into the container at /app
# ADD . /app

# Install any needed packages specified in requirements.txt
# RUN dnf -y install make gcc g++ cmake git boost clang vim bash cppcheck tmux
RUN dnf -y install make gcc g++ cmake git boost bash rpm-build && dnf clean all
RUN git clone https://github.com/kracejic/dotfiles-minimal.git ~/bin && cd ~/bin && ./install.sh

# Make port 80 available to the world outside this container
# EXPOSE 80

# Define environment variable
# ENV NAME World

# Run app.py when the container launches
CMD ["bash"]

