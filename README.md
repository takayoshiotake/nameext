# nameext

## Installation

https://github.com/takayoshiotake/homebrew-tap

```
$ brew tap takayoshiotake/tap
$ brew install nameext
```

## Usage

```
$ nameext
usage: nameext [-h] {add,rm} ...

Filename extension manipulation tool

positional arguments:
  {add,rm}
    add       Add extension
    rm        Remove extension

optional arguments:
  -h, --help  show this help message and exit
$ nameext add
usage: nameext add [-h] extension file
nameext add: error: the following arguments are required: extension, file
$ nameext rm
usage: nameext rm [-h] file
nameext rm: error: the following arguments are required: file
```

e.g.

```
$ ls
test.txt
$ nameext add bak test.txt
$ ls
test.txt.bat
$ nameext rm *.txt
$ ls
test.txt
$ nameext rm *
$ ls
test
```
