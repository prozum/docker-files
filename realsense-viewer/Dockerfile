FROM nvidia/opengl:1.0-glvnd-devel-ubuntu18.04

RUN apt-get update
RUN apt-get install --no-install-recommends -y gnupg2 software-properties-common
RUN apt-key adv --keyserver keys.gnupg.net --recv-key 6F3EFCDE
RUN add-apt-repository "deb http://realsense-hw-public.s3.amazonaws.com/Debian/apt-repo bionic main" -u
RUN apt-get install --no-install-recommends -y librealsense2-utils 
RUN rm -rf /var/lib/apt/lists/*
