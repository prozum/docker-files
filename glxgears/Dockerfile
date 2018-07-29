FROM ubuntu:18.04

RUN apt-get update
RUN apt-get install --no-install-recommends -y libglvnd0 mesa-utils
RUN rm -rf /var/lib/apt/lists/*

ENV NVIDIA_VISIBLE_DEVICES ${NVIDIA_VISIBLE_DEVICES:-all}
ENV NVIDIA_DRIVER_CAPABILITIES ${NVIDIA_DRIVER_CAPABILITIES:+$NVIDIA_DRIVER_CAPABILITIES,}graphics
