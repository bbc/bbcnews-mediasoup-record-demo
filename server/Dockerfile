FROM node:14

WORKDIR /home/node/server

COPY . .

RUN apt-get update

RUN apt-get -y install ffmpeg
RUN ffmpeg -version

RUN apt-get -y install libgstreamer1.0-0 
RUN apt-get -y install gstreamer1.0-plugins-base
RUN apt-get -y install gstreamer1.0-plugins-good
RUN apt-get -y install gstreamer1.0-plugins-bad
RUN apt-get -y install gstreamer1.0-plugins-ugly 
RUN apt-get -y install gstreamer1.0-libav 
RUN apt-get -y install gstreamer1.0-doc 
RUN apt-get -y install gstreamer1.0-tools 
RUN apt-get -y install gstreamer1.0-x 
RUN apt-get -y install gstreamer1.0-alsa
RUN apt-get -y install gstreamer1.0-pulseaudio

# RUN apt-get -y install gstreamer1.0-gl
# RUN apt-get -y install gstreamer1.0-gtk3
# RUN apt-get -y install gstreamer1.0-qt5

RUN npm install

CMD [ "node", "src/server" ]

