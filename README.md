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

Then, you can download it using the download link.

linux example

```bash
wget -O go2 https://github.com/myyrakle/go2/releases/download/go2-1.22.6/go-1-22-6-linux-amd64
sudo chmod +x go2
export GO_FILE_PATH=$(which go)

if [ -L "$GO_FILE_PATH" ]; then
    echo "$GO_FILE_PATH is symbolic link"
    export GO_FILE_PATH=$(readlink -f $GO_FILE_PATH)
fi

sudo mv $GO_FILE_PATH "$GO_FILE_PATH-old"
sudo mv go2 $GO_FILE_PATH
sudo chmod 777 $GO_FILE_PATH
```

If the replacement is done without problems, it should run fine.
![image](https://github.com/user-attachments/assets/dbac61d0-7721-4cc9-a181-f6563f609738)

