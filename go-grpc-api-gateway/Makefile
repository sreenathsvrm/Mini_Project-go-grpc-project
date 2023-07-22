# proto:
# proto target compiles the protocol buffer files for authentication, order, and product packages.
# It uses the 'protoc' command to generate gRPC code from the .proto files.
# The generated code will be placed in the same directory as the .proto files.
# Compiling auth.proto
proto:
	protoc pkg/auth/pb/*.proto --go_out=plugins=grpc:.
	protoc pkg/order/pb/*.proto --go_out=plugins=grpc:.
	protoc pkg/product/pb/*.proto --go_out=plugins=grpc:.

server:
# server target runs the main.go file to start the server.
# Starting the server
	go run cmd/main.go