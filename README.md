# scout_i386-resources

TODO: More in depth explanation

To install gcc-12:

```
wget https://github.com/Octoshark/scout_i386-resources/releases/download/v0.0.1/gcc12.tar.gz
tar xf gcc12.tar.gz -C /
```

To install CMake:

```
wget https://github.com/Octoshark/scout_i386-resources/releases/download/v0.0.1/cmake-3.24.0-rc5-i386.tar.gz
tar xf cmake-3.24.0-rc5-i386.tar.gz -C /usr
```

To add binutils 2.30 to PATH:

```
echo "export PATH=\"/usr/lib/binutils-2.30/bin:\$PATH\"" >> /root/.bashrc
```

Alternatively, use the docker container:

```
docker pull spirrwell/pvkii-scout-i386
docker run -it --entrypoint /bin/bash -v $PWD:/build -w /build --rm spirrwell/pvkii-scout-i386
```
