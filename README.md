# 개발 환경
Windows Docker Desktop
Visual Studio Code
- Remote-Container
- ctrl+shift+p
- remote-containers: clone repository in container volume
- https://github.com/philosup/go-with-grpc
- unique
- GO


# gRPC Go Quick Start
https://grpc.io/docs/languages/go/quickstart/


## module
```bash

go mod init philosup/go-with-grpc


go get google.golang.org/grpc
# go get google.golang.org/grpc/cmd/protoc-gen-go-grpc
# go get google.golang.org/protobuf/cmd/protoc-gen-go
go get github.com/golang/protobuf/protoc-gen-go
```
```
protoc --go_out=plugins=grpc:. helloworld.proto
```
## protoc 설치

### 윈도우
https://github.com/protocolbuffers/protobuf/releases/
https://github.com/protocolbuffers/protobuf/releases/download/v3.14.0/protoc-3.14.0-win64.zip

GOPATH/bin으로 복사해서 사용.
또는
압축해제한 폴더

###  linux
```sh
sudo apt update
sudo apt install protobuf-compiler -y
```
