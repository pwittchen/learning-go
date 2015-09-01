# learning-go
Repository created in order to learn basics of Go language

Installation on Linux
---------------------

Official download website: https://golang.org/dl/

Download go and extract it to `/usr/local/` directory:

```
$ wget https://storage.googleapis.com/golang/go1.5.linux-amd64.tar.gz
$ sudo tar -C /usr/local -xzf go1.5.linux-amd64.tar.gz
```

Set environmental variables in your `.zshrc` or `.bashrc` file:

```
export PATH=$PATH:/usr/local/go/bin
export GOPATH=$HOME/Development/go/workspace
export GOBIN=$GOPATH/bin
```

Compiling and running programs
------------------------------

Create the following program with name `hello.go`:

```go
package main

import "fmt"

func main() {
    fmt.Printf("hello, world\n")
}
```

Start terminal and compile the program:

```
go install hello.go
```

Run the program:

```
$ $GOBIN/hello
```

References
----------
- [Official Go website](https://golang.org)
- [Getting started](https://golang.org/doc/install)
