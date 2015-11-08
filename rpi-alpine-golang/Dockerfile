FROM armbuild/alpine

MAINTAINER Constantin Clauzel < constantin.clauzel@gmail.com >

RUN 	apk update && \
	apk add curl && \
	apk add gcc && \
	apk add make && \
	apk add bash && \
	apk add musl-dev && \
	curl http://dave.cheney.net/paste/go-linux-arm-bootstrap-c788a8e.tbz | tar xj && \
	curl https://storage.googleapis.com/golang/go1.5.src.tar.gz | tar xz && \
	cd /go/src/ && \
	GOROOT_BOOTSTRAP=/go-linux-arm-bootstrap ./make.bash && \
	cp /go/bin/go /usr/local/bin/ && \
	cp /go/bin/gofmt /usr/local/bin/
	

RUN mkdir gopath

ENV GOPATH /gopath

ENTRYPOINT ["/bin/bash"]
