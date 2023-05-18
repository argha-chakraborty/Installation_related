Download the Python-3.xx.xx.tar.xz from the [official website](https://www.python.org/downloads/) and move to the directory named "softwares"

```bash
cd softwares
```
Untar the Python-3.xx.xx.tar.xz file

```bash
tar -xvf Python-3.xx.xx.tar.xz
```
```bash
cd Python-3.xx.xx
```

Configure the build in the "build-location/python3"

```bash
./configure --prefix=build-location/python3 --exec-prefix=build-location/python3 --enable-shared
```
```bash
make -j 10
```
```bash
make install
```
Installation is complete
