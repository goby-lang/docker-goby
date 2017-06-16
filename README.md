# docker-goby

## Usage

### Pull Image

```
$ docker pull st0012/goby:latest
```

### Execute File

```
# In container, default working directory is /go/src/github.com/goby-lang/goby 
$ docker run -t -v PATH_TO_TARGET_FILE_DIR:/go/src/github.com/goby-lang/goby st0012/goby:latest goby TARGET_FILE
```

For example if I want to run `./samples/loop.gb`, I will run

```
$ docker run -t -v `pwd`/samples:/go/src/github.com/goby-lang/goby st0012/goby:latest goby loop.gb
```
