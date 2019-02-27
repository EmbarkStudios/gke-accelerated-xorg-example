FROM ubuntu:bionic
EXPOSE 5900
ENV DEBIAN_FRONTEND noninteractive
RUN apt-get update -qy && \
    apt-get install -qy --no-install-recommends \
      dwm mesa-utils x11vnc xinit xterm xserver-xorg
COPY xorg.conf /etc/X11/xorg.conf
COPY run /usr/bin/run
ENTRYPOINT ["/usr/bin/run"]
CMD []
