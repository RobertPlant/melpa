FROM debian:stable-20230227-slim

RUN apt-get update
RUN DEBIAN_FRONTEND=noninteractive apt-get --yes install curl emacs-nox git make mercurial ruby texinfo imagemagick && \
        apt-get clean && rm -rf /var/lib/apt/lists/
WORKDIR /mnt/store/melpa
CMD docker/builder/run.sh
