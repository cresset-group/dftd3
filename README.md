# DFT-D3

A dispersion correction for density functionals, Hartree-Fock and semi-empirical quantum chemical methods DFT-D3.

Taken from https://www.chemie.uni-bonn.de/pctc/mulliken-center/software/dft-d3/.

Windows support has been added and the build system switched to CMake.

# Build

## Windows
```
mkdir build
cd build
cmake -DCMAKE_Fortran_COMPILER=ifort -DCMAKE_INSTALL_PREFIX=install -G "NMake Makefiles" ..
nmake
nmake install
```
## Linux
```
mkdir build
cd build
cmake3 -DCMAKE_Fortran_COMPILER=ifort -DCMAKE_INSTALL_PREFIX=install -G "Unix Makefiles" ..
make
make install
```
