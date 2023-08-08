# Installation of Openmpi for launching parallel process

1. Install gcc for all machines, run:

   ```bash
   sudo apt-get install gcc
   ```
   ```bash
   sudo apt-get install openmpi-bin openmpi-common libopenmpi-dev libgtk2.0-dev
   ```
2. Download the openmpi-4.x.x.tar.gz file from [official website](https://www.open-mpi.org/software/ompi/v4.1/) and move to desired directory say 'softwares'
   Untar the file

   ```bash
   tar -zxvf openmpi-4.x.x.tar.gz
   ```
   ```bash
   cd openmpi-4.x.x
   ```
3. Install openmpi
   ```bash
   ./configure --prefix="/path/to/prefix/openmpi"
   ```
   ```bash
   make
   ```
   ```bash
   make install
   ```
4. Export path

   ```bash
   export PATH="$PATH:/path/to/prefix/openmpi/bin"
   ```
   ```bash
   export LD_LIBRARY_PATH="$LD_LIBRARY_PATH:/path/to/prefix/openmpi/lib"
   ```
   
   
