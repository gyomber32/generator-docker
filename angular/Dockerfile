FROM node:10

RUN apt-get install git
RUN apt-get install -y curl
RUN npm install -g @angular/cli --unsafe

RUN echo "Changed to /home/ginger/Szakdolgozat/generator-docker"
WORKDIR /home/ginger/Szakdolgozat/generator-docker

RUN echo "Git clone done"
RUN git clone https://github.com/gyomber32/angular2-generator-gui.git

RUN echo "Changed to /home/ginger/Szakdolgozat/generator-docker/angular2-generator-gui"
WORKDIR /home/ginger/Szakdolgozat/generator-docker/angular2-generator-gui

RUN echo "Running npm install"
RUN npm install

EXPOSE 4200

RUN echo "Starting generator-angular"
CMD ng serve --aot --host 0.0.0.0
