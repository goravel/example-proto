# example-proto

Provide proto for goravel/example

```shell
# 1. Install Protocol Tools

- [protoc@libprotoc](https://grpc.io/docs/protoc-installation/): Generate proto files.
  - check the version by `protoc --version`
- [protoc-gen-go](https://grpc.io/docs/languages/go/quickstart/#prerequisites): Generate go files from proto files.
  - `go install google.golang.org/protobuf/cmd/protoc-gen-go@latest`
  - check the version by `protoc-gen-go --version`
- [protoc-gen-go-grpc](https://grpc.io/docs/languages/go/quickstart/#prerequisites): Generate go grpc files from proto 
  files.
  - `go install google.golang.org/grpc/cmd/protoc-gen-go-grpc@latest`
  - check the version by `protoc-gen-go-grpc --version`

# 2. Generate proto files
protoc --go_out=. --go-grpc_out=. *.proto
```
