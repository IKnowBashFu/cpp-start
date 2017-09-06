# CPP Start

A repository for quickly getting a simple C++ project off the ground.

#### Requirements

* gcc
* make

#### Installation (On Ubuntu)
```sh
sudo apt-get install build-essentials git
mkdir -p ~/Code/c && cd ~/Code/c
git clone https://github.com/ChrisVollink/cpp-start.git template
cd template && make
bin/hello
```

If everything went well (why wouldn't it) you should see this output:

```
$ make
 g++ -g -Wall -I include -c -o build/hello.o src/hello.cpp
 g++ -g -Wall -I include -c -o build/util.o src/util.cpp
 Linking...
 g++ build/hello.o build/util.o -o bin/hello
$ bin/hello
Hello, World!
```

You could also use clang, if you prefer, by running

```
$ make CC=clang++
```
