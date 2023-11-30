.PHONY: proto
proto: ./proto/book/catalogue.proto
	cd ./proto/book && protoc \
		--go_out=. \
		--go_opt=paths=source_relative \
		--go-grpc_out=. \
		--go-grpc_opt=paths=source_relative \
		catalogue.proto

.PHONY: clean
clean:
	rm -f ./proto/book/*.go

.PHONY: run
run:
	go run ./main.go