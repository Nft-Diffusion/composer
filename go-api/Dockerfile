FROM golang:latest 

RUN mkdir /build 
WORKDIR /build 

RUN export GO111MODULE=on 

RUN go get github.com/URL 
RUN cd /build && git clone https://github.com/URL.git 

RUN cd /build/GoWebApi/main && go build 

EXPOSE 8080 

ENTRYPOINT ["/build/GoWebAPI/index"]