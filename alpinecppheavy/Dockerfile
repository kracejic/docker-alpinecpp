FROM alpine

# Set the working directory to /app
# WORKDIR /app

# Copy the current directory contents into the container at /app
# ADD . /app

# Install any needed packages specified in requirements.txt
RUN apk update
RUN apk add make gcc g++ cmake git boost-dev clang vim bash cppcheck tmux
RUN git clone https://github.com/kracejic/dotfiles-minimal.git ~/bin && cd ~/bin && ./install.sh

# Make port 80 available to the world outside this container
# EXPOSE 80

# Define environment variable
# ENV NAME World

# Run app.py when the container launches
CMD ["bash"]

