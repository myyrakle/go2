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

## Install from Github Release

First, check the previously installed go version. 

![image](https://github.com/user-attachments/assets/629a0749-53de-46ba-94de-af09c0072ee0)

And in release, we find a match between the minor version and the OS.

linux example
```bash
sudo rm -rf /usr/local/go && sudo tar -C /usr/local -xzf linux_amd64.tar.gz
```

If the replacement is done without problems, it should run fine.
![image](https://github.com/user-attachments/assets/dbac61d0-7721-4cc9-a181-f6563f609738)

