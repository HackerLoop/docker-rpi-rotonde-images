FROM armbuild/alpine

MAINTAINER Constantin Clauzel < constantin.clauzel@gmail.com >

RUN 	apk update && \
	apk add libusb

ADD rotonde-barcode-lv4500 /
ADD libs/* /usr/local/lib/

ENTRYPOINT ["/rotonde-barcode-lv4500"]
