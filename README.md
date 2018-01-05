# docker-protoc
Docker image with protobuf compiler and various language plugins

## Usage
```
$ docker run --rm gwihlidal/protoc --help
Usage: /usr/bin/protoc [OPTION] PROTO_FILES
```

```
$ docker run --rm -v $(pwd):$(pwd) -w $(pwd) gwihlidal/protoc --cpp_out=. -I. your.proto
```

## Supported languages and tools
- C
- C++
- C#
- Rust
- Python
- Ruby
- Go
- Java / JavaNano
- JavaScript
- Objective-C
- Swift 4
- Swagger
- grpc-gateway

## Google Types
Google well known types are embedded and `protoc` will include them automatically.
https://developers.google.com/protocol-buffers/docs/reference/google.protobuf

The types are available in `google/protobuf/`:
```protobuf
syntax = "proto3";
import "google/protobuf/timestamp.proto";
```

## Versions
- grpc: 1.7.2
- grpc_java: 1.8.0
- protobuf: 3.5.1
- protobuf-c: 1.3.0
- swift: 4.0.3
- llvm: 5.0.0
- swift-protobuf: 1.0.2
- rust-protobuf: 1.4.3
- go: 1.9.2

## Repositories
- https://github.com/google/protobuf
- https://github.com/grpc
- https://github.com/grpc/grpc-java
- https://github.com/protobuf-c
- https://github.com/Masterminds/glide
- https://github.com/golang/protobuf/protoc-gen-go
- https://github.com/gogo/protobuf/protoc-gen-gofast
- https://github.com/gogo/protobuf/protoc-gen-gogo
- https://github.com/gogo/protobuf/protoc-gen-gogofast
- https://github.com/gogo/protobuf/protoc-gen-gogofaster
- https://github.com/gogo/protobuf/protoc-gen-gogoslick
- https://github.com/grpc-ecosystem/grpc-gateway/protoc-gen-swagger
- https://github.com/grpc-ecosystem/grpc-gateway/protoc-gen-grpc-gateway
- https://github.com/johanbrandhorst/protobuf/protoc-gen-gopherjs
- https://github.com/ckaznocha/protoc-gen-lint
- https://github.com/pseudomuto/protoc-gen-doc
- https://github.com/apple/swift-protobuf
- https://github.com/stepancheg/rust-protobuf
- http://releases.llvm.org
- https://swift.org
