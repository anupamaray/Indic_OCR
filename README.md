# Indic_OCR
OCR software for Indian languages


Installation:

This code has been written in C++ and tested on Ubuntu 12.04. However it should run on any linux platform. This code needs the following for compilation.

A modern C++ compiler (e.g. gcc 3.0 or higher)
Install opencv
automake 1.9 install from software centre
libtool install from software centre

Install following Python packages: 
sudo apt-get install python-scipy python-numpy python-matplotlib
sudo apt-get install python-pip
pip install PIL

Install java:
sudo apt-get install openjdk-7-jdk

Download rnnlib and other tar files for netcdf, ScientificPython(not scipy) and boost(headers reqd only): all tar attached

tar -xvf netcdf-4.0.tar.gz
tar -xvf ScientificPython-2.8.1.tar.gz

Installing Boost libraries:

cd Downloads/boost_1_59_0/
./bootstrap.sh
sudo ./b2
sudo ./b2 install

--------------------------------------

Installing netcdf:

cd netcdf-4.0/
CFLAGS=-fpic ./configure
sudo make install
make check

--------------------------------------------
for netCDF operator: install nco from software centre

Installing ScientificPython:

cd ScientificPython-2.8.1/
sudo python setup.py build
sudo python setup.py install
 
--------------------------------------------


Installing RNNLIB:

cd rnnlib/rnnlib_source_forge_version
CXXFLAGS=-I/usr/local/include/boost/ ./configure
sudo make
----------------------------------------

In the given folder OriyaOCR, there is a folder models, copy the model file from this folder and paste it in utils folder which can be found in: rnnlib/rnnlib_source_forge_version/utils/

To test:
run: ./Aksharayan_Oriya input.xml output.xml 1.txt


Please feel free to contact@ anupamaray88@gmail.com for any queries
