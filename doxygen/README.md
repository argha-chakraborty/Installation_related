Download the source code file from the [official website](https://www.doxygen.nl/download.html) and move it to the desired directory "softwares"

```bash
cd softwares
```
Untar the doxygen-1.x.x.xxx.tar.xf file

```bash
tar -xvf doxygen-1.x.x.xxx.tar.xf
```
```bash
cd doxygen-1.x.x.xxx
```
Create a build directory

```bash
mkdir build
```
```bash
cd build
```

Now to install with a specified python version in a specified build-location/doxygen-1.x.x

```bash
cmake ../ -DCMAKE_INSTALL_PREFIX=build-location/doxygen-1.x.x -DPYTHON_EXECUTABLE=specified-python-location/python3/bin/python3
```
```bash
make -j 10
```
```bash
make install
```

Installation is complete
