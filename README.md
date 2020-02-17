# vala-lib-example

A complete example of a Vala library and consumer projects using Meson.  This demonstrates the code and build files needed to produce and consume a library in Vala.

## Build

### Library

```bash
$ cd lib-producer
$ meson build
$ cd build
$ ninja install
```

### Consuming App

```bash
$ cd app-consumer
$ meson build
$ cd build
$ ninja
$ ./app-consumer
my math: 4
```