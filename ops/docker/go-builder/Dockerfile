FROM golang:1.18.0-alpine3.15

RUN apk add --no-cache make gcc musl-dev linux-headers git jq curl bash gzip ca-certificates openssh && \
	go install gotest.tools/gotestsum@latest && \
	curl -sSfL https://raw.githubusercontent.com/golangci/golangci-lint/master/install.sh | sh -s -- -b $(go env GOPATH)/bin v1.45.2

CMD ["bash"]
