# cloud-native-ms-dev-ops

## Setup

### Go

- https://go.dev/dl/
- Installer
- M1 Mac: go${version}.darwin-arm64.pkg

```shell
go version
```
 
## Protocol Buffers

```shell
brew install protobuf
protobuf --version
```

## Plugins for Protocol Buffers

```shell
go install google.golang.org/protobuf/cmd/protoc-gen-go@v1.28 
go install google.golang.org/grpc/cmd/protoc-gen-go-grpc@v1.2
echo 'export PATH="$PATH:'$(go env GOPATH)'/bin"' >> ~/.zshrc
source ~/.zshrc
```

## Node.js

```shell
brew install node
node --version
```
## Docker

## kubectl

```shell
brew install kubectl
kubectl version --client
```

## kind

```shell
brew install kind
kind --version
```

## istioctl

https://istio.io/latest/docs/setup/getting-started/#download

```shell
mkdir ~/opt
cd ~/opt
curl -L https://istio.io/downloadIstio | sh -
cd istio-<version>/bin
echo 'export PATH="$PATH:'$PWD'"' >> ~/.zshrc
source ~/.zshrc
```