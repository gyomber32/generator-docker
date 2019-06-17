FROM node

RUN echo "Changed to /home/ginger/Szakdolgozat/generator-docker"
WORKDIR /home/ginger/Szakdolgozat/generator-docker

RUN echo "Git clone done"
RUN git clone https://github.com/gyomber32/generator-loopback.git

RUN echo "Changed to /home/ginger/Szakdolgozat/generator-docker/generator-loopback"
WORKDIR /home/ginger/Szakdolgozat/generator-docker/generator-loopback

RUN echo "Running npm install"
RUN npm install

RUN echo "Starting generator-loopback"
CMD node .
