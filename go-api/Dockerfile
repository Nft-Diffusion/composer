FROM golang:latest 

ADD . /go/src/github.com/Nft-Diffusion/api
RUN go install github.com/Nft-Diffusion/api@v1.0.0

ENTRYPOINT /go/bin/api

EXPOSE 3000