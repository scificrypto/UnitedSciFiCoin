# Dockerfile for building unitedscifi binaries.

Now, you can build your own unitedscifi files on all systems with docker and do it easy without installing depends on your system.

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
sudo docker run -it -v ~/path/to/unitedscifi/folder:/unitedscifi 9bbff825d50f
```

If your system uses SELINUX you may use --privileged=true key

```
sudo docker run --privileged=true -it -v ~/development/unitedscifi:/unitedscifi 9bbff825d50f
```

See unitedscifi-qt file in used unitedscifi folder and unitedscifid file in src subfolder.