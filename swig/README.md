Download the source code file swig.4.x.x.tar.gz file from [official website](https://www.swig.org/download.html) and move it to the desired directory "softwares"

```bash
cd softwares
```
Untar the swig.4.x.x.tar.gz file

```bash
tar -xvf swig.4.x.x.tar.gz
```
```bash
cd swig.4.x.x
```

Now to install swig in a desired "build-location/swig" with a specified python
```bash
./configure --prefix=build-location/swig --with-python=specified-python-path/python3/bin/python3
```
```bash
make -j 10
```
```bash
make install
```

Installation is complete
