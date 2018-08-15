# hello-senzing

## Usage

A simple program to show how to use senzing
[senzing](https://senzing.com/).

### Invocation

```console
hello-senzing
```

## Demonstrate

### Terminal #1


## Development

### Dependencies

#### Set environment variables

```console
export GOPATH="${HOME}/go"
export PATH="${PATH}:${GOPATH}/bin:/usr/local/go/bin"
export PROJECT_DIR="${GOPATH}/src/github.com/docktermj"
export REPOSITORY_DIR="${PROJECT_DIR}/go-hello-etcd"
```

#### Download project

```console
mkdir -p ${PROJECT_DIR}
cd ${PROJECT_DIR}
git clone git@github.com:docktermj/go-hello-etcd.git
```

#### Download dependencies

```console
cd ${REPOSITORY_DIR}
make dependencies
```

Etcd command-line tool

```console
go get -u github.com/coreos/etcd/etcdctl
```

Fix [bug](https://github.com/coreos/etcd/issues/8715).

```console
rm  ${REPOSITORY_DIR}/vendor/github.com/coreos/etcd/client/keys.generated.go
```

### Build

#### Local build

```console
cd ${REPOSITORY_DIR}
make
```

The results will be in the `${GOPATH}/bin` directory.

#### Docker build

Create `rpm` and `deb` installation packages.

```console
cd ${REPOSITORY_DIR}
make build
```

The results will be in the `${REPOSITORY_DIR}/target` directory.

### Test

```console
cd ${REPOSITORY_DIR}
make test-local
```

### Cleanup

```console
cd ${REPOSITORY_DIR}
make clean
```
