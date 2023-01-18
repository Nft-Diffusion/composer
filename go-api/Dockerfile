FROM golang:latest 

RUN mkdir /build 
WORKDIR /build 

RUN export GO111MODULE=on 

RUN go get https://github.com/Nft-Diffusion/api
RUN cd /build && git clone https://github.com/Nft-Diffusion/api.git
# RUN cd /build/api && go mod download && go mod verify 
RUN cd /build/api && go build 

EXPOSE 8080 

ENTRYPOINT ["/build/index"]