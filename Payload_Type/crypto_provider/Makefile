.PHONY: build test run

build:
	CGO_ENABLED=0 go build -buildvcs=false -trimpath -o .build/crypto-provider .

test:
	go test -race ./...

run: build
	.build/crypto-provider
