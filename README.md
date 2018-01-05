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
