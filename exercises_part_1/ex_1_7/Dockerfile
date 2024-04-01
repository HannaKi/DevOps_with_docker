# Start from the ubuntu image
FROM ubuntu:22.04

# Use /usr/src/app as our workdir. The following instructions will be executed in this location.
WORKDIR /usr/src/app

# install curl inside the container: 
RUN apt-get update
RUN apt-get -y install curl

# Copy the scritp.sh file from this directory to /usr/src/app/ creating /usr/src/app/script.sh
COPY script.sh .

# Add execution permissions during the build.
RUN chmod +x script.sh

# When running docker run the command will be ./script.sh
CMD ./script.sh
