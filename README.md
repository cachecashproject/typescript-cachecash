# TypeScript-Cachecash


TypeScript-Cachecash is a web application to demonstrate different usages of CacheCash.

## You need to get Go-Cachecash up and running for TypeScript-Cachecash
Go to [Go-Cachecash] and follow the README to set up Go-Cachecash.

[Go-Cachecash]: https://github.com/cachecashproject/go-cachecash

## Cloning the git repository

```bash
git clone git@github.com:cachecashproject/typescript-cachecash.git 
```

## Installing Dependencies

Please make sure you have installed [Node.js], [llvm], [rustup], [wasm-pack]

[Node.js]: https://nodejs.org/en/
[llvm]: https://llvm.org/docs/CMake.html
[rustup]: https://rustup.rs/
[wasm-pack]: https://rustwasm.github.io/wasm-pack/

## Building Docker Image


`You should already have Go-cachecash tested at this point`
Build the latest docker image by:
```bash
docker build -t typescript-cachecash .
```


## Running TypeScript-Cachecash

First go to go-cachecash folder, start the containers:

```bash
docker-compose up -d
```

Then go back to typescript folder and start the typescript container:

```bash
docker run -p 127.0.0.1:1234:1234 --name typescript-cachecash-daemon -t typescript-cachecash
```

Then you can check out the sites to explore what cachecash can do:

Cachecash basic functionalities:

127.0.0.1:1234/demo/basic

Watch a video served by caches:

127.0.0.1:1234/demo/pigduckbunny

Download a file served by caches:

127.0.0.1:1234/demo/html5-download
