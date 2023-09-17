.DEFAULT_GOAL := build

fmt:
    go fmt ./...
.PHONY: fmt

lint: fmt
    golint ./...
.PHONY: lint

vet: fmt
    go vet ./...
.PHONY: vet

build: vet
    go build hello.go
.PHONY: build

# hello:
# 	echo "hello"

# build:
# 	go build hello.go

# run:
# 	go run hello.go