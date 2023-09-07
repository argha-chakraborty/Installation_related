OpenMM has dependency on Python, Cmake, Doxygen and Swig 

Install [Python3](https://github.com/argha-chakraborty/Installation_related/tree/main/Python3); [Cmake](https://github.com/argha-chakraborty/Installation_related/tree/main/cmake); [Doxygen](https://github.com/argha-chakraborty/Installation_related/tree/main/doxygen) and [Swig](https://github.com/argha-chakraborty/Installation_related/tree/main/swig)


Clone the OpennMM source code from [github-page](https://github.com/openmm/openmm) and move it to the desired directory "softwares"

```bash
cd softwares
```
Unzip openmm-master.zip file 

```bash
unzip openmm-master.zip
```
```bash
cd openmm-master
```
create a build directory
```bash
mkdir build
```
```bash
cd build
```
Now install OpenMM for CUDA with a specified python in a specified build-location

```bash
installed-path/cmake/bin/cmake ../ -DPYTHON_EXECUTABLE=installed-path/python3/bin/python3 -DCMAKE_INSTALL_PREFIX=build-location/openmm -DSWIG_EXECUTABLE=installed-path/swig/bin/swig -DCUDA_TOOLKIT_ROOT_DIR=/usr/local/cuda -DOPENMM_BUILD_SHARED_LIB=ON -DOPENMM_BUILD_STATIC_LIB=ON -DOPENMM_BUILD_C_AND_FORTRAN_WRAPPERS=ON -DBUILD_TESTING=ON -DOPENMM_BUILD_CUDA_LIB=ON -DOPENMM_BUILD_OPENCL_LIB=OFF -DOPENMM_BUILD_CPU_LIB=ON -DOPENMM_BUILD_AMOEBA_PLUGIN=ON -DOPENMM_BUILD_RPMD_PLUGIN=ON -DOPENMM_BUILD_DRUDE_PLUGIN=ON -DOPENMM_BUILD_PME_PLUGIN=ON
```

To install OpenMM without CUDA with a specified python in a specified build-location
```bash
installed-path/cmake/bin/cmake ../ -DPYTHON_EXECUTABLE=installed-path/python3/bin/python3 -DCMAKE_INSTALL_PREFIX=build-location/openmm -DSWIG_EXECUTABLE=installed-path/swig/bin/swig -DDOXYGEN_EXECUTABLE=installed-path/doxygen/bin/doxygen -DOPENMM_BUILD_SHARED_LIB=ON -DOPENMM_BUILD_STATIC_LIB=ON -DOPENMM_BUILD_C_AND_FORTRAN_WRAPPERS=ON -DBUILD_TESTING=ON -DOPENMM_BUILD_CUDA_LIB=OFF -DOPENMM_BUILD_OPENCL_LIB=OFF -DOPENMM_BUILD_CPU_LIB=ON -DOPENMM_BUILD_AMOEBA_PLUGIN=ON -DOPENMM_BUILD_RPMD_PLUGIN=ON -DOPENMM_BUILD_DRUDE_PLUGIN=ON -DOPENMM_BUILD_PME_PLUGIN=ON
```
```bash 
make -j 20
```
```bash
make install
```
```bash
make PythonInstall
```
```bash
export PATH=$PATH:installed-path/python3/lib/python3/dist-packages/simtk
```
```bash
make test
```
Copy simtk folder to the build-location/openmm folder

```bash
cp -r build/python/build/lib.linux-x86_64-cpython-39/simtk build-location/openmm
```
