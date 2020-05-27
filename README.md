# bzip2cgo

build in ubuntu:

```bash
apt-get install -y libbz2-dev
```

and then:

```bash
cd bzipper
go build -v .
```

try:

```bash
# compress and decompress
< main.go ./bzipper | bunzip2 | sha1sum

# verify
cat main.go | sha1sum
```
