API_PROTO_FILES=$(shell find v1 -name *.proto)

default:api

.PHONY: api
# generate api proto
api:
	protoc --proto_path=./v1 \
 	       --go_out=paths=source_relative:./v1 \
 	       --go-grpc_out=paths=source_relative:./v1 \
	       $(API_PROTO_FILES)