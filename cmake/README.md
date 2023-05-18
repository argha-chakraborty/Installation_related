Download the desired linux version of tar file from the [official website](https://cmake.org/download/) and move it to the source build directory named "softwares"

```bash
cd softwares
```
Untar the cmake-3.xx.x-linux-x86_64.tar.gz file 

```bash
tar -xvf cmake-3.xx.x-linux-x86_64.tar.gz
```

Now to install in specified directory "build-location/cmake"

```bash
./bootstrap --prefix=/path/to/prefix/cmake
```
```bash
make -j 10
```
```bash
make install
```
Installation is complete
