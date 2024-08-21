# The Go2 Programming Language

A radical fork version of Go Compiler


[Original README](./old.README.md)


## changes

1. Eliminates all concurrent map write&read panics.

## Install from Source

```bash 
export PROJECT_ROOT=$(pwd)
cd src 
GOROOT_BOOTSTRAP=$PROJECT_ROOT/bin ./make.bash
```

windows
```bash
export GOOS=windows 
export GOARCH=amd64
```

linux
```bash
export GOOS=linux 
export GOARCH=amd64
```

macos
```bash
export GOOS=darwin 
export GOARCH=arm64
```