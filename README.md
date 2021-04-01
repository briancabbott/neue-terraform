# neue-terraform
New Terraform for TrueMark! Bigger, Better, More Power[ful]! 


# Build Notes

The main first step is to have a complete stand-alone build of Terraform, then we can begin dismantalling it!

Steps:
   - 0. Ensure go-lang setup:
      - 0.1: GOROOT: export GOROOT=/usr/local/go 
      - 0.2: GOPATH: export GOPATH=~/go
      - 0.3: PATH: export PATH=$PATH:$GOPATH/bin
      - 0.4: Go Modules: export GO111MODULE=on 
   - 1. Install protobuf, protobuf-gen-go:
```
go get google.golang.org/protobuf/cmd/protoc-gen-go@latest
go get google.golang.org/grpc/cmd/protoc-gen-go-grpc

go install google.golang.org/protobuf/cmd/protoc-gen-go@latest
go install google.golang.org/grpc/cmd/protoc-gen-go-grpc

go: downloading google.golang.org/protobuf v1.26.0
➜  neue-terraform 
```
 