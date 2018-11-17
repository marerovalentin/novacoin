# Dockerfile for building nodcoin binaries.

Now, you can build your own nodcoin files on all systems with docker and do it easy without installing depends on your system.

## How:

### Build docker image

```
sudo docker build .
```

### Run docker container

Builder will return HASH of image
Example:
Successfully built 9bbff825d50f

```
sudo docker run -it -v ~/path/to/nodcoin/folder:/nodcoin 9bbff825d50f
```

If your system uses SELINUX you may use --privileged=true key

```
sudo docker run --privileged=true -it -v ~/development/nodcoin:/nodcoin 9bbff825d50f
```

See nodcoin-qt file in used nodcoin folder and nodcoind file in src subfolder.