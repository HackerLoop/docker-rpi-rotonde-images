FROM armbuild/alpine

MAINTAINER Constantin Clauzel < constantin.clauzel@gmail.com >

RUN 	apk update && \
	apk add curl && \
	apk add gcc && \
	apk add make && \
	apk add bash && \
	apk add musl-dev && \
	apk add git && \
	apk add autoconf && \
	apk add automake && \
	apk add libtool && \
	apk add eudev-libs eudev-dev && \
	apk add libusb libusb-dev && \
	apk add linux-headers
	
RUN mkdir /sources

VOLUME sources

ENTRYPOINT ["/bin/bash"]
