#
# SQLite Browser
#
# USAGE :
#   docker run -d \
#     --net host \
#     -v /tmp/.X11-unix:/tmp/.X11-unix \
#     -v $HOME/.sqlitebrowser:/root/sqlitebrowser \
#     -e DISPLAY=unix$DISPLAY \
#     --name sqlitebrowser \
#     portiad/sqlitebrowser


FROM ubuntu:latest
MAINTAINER Portia Dean

ENV DEBIAN_FRONTEND noninteractive

RUN apt-get update && apt-get install -y \
	sqlite3 \
	libsqlite3-dev \
	sqlitebrowser \
	software-properties-common

CMD sqlitebrowser