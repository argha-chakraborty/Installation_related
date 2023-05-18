Download the LINUX version file from [official website](https://www.ks.uiuc.edu/Development/Download/download.cgi?PackageName=VMD) and move to desired directory say 'softwares'

```bash
cd softwares
```
untar the source code file in the same directory

```bash
tar -xf vmd-1.x.xxx.xxxxx.tar.gz
```

Configure the build in the same directory

```bash
./configure
```

Next you'll need to make the dependency list INSIDE THE SRC DIRECTORY

```bash
cd src
```
Now to install

```bash
sudo make install
```
VMD installation complete. Enjoy!!
