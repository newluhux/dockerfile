FROM alpine:edge

RUN echo 'https://dl-cdn.alpinelinux.org/alpine/edge/testing' >> /etc/apk/repositories
RUN sed -i -e 's/dl-cdn.alpinelinux.org/mirrors.bfsu.edu.cn/g' /etc/apk/repositories

RUN apk update && \
	apk add -v qt-creator build-base musl-dbg gdb \
		clang-extra-tools strace valgrind cmake git \
		qt5-qtbase-dev qt6-qtbase-dev \
		qt5-qtbase-dbg qt6-qtbase-dbg \
		qt5-qtwayland-dev qt6-qtwayland-dev \
		qt5-qtwebsockets-dev qt6-qtwebsockets-dev \
		qt5-qtserialport-dev qt6-qtserialport-dev \
