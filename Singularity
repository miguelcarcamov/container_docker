BootStrap: docker
From: nvidia/cuda:10.1-cudnn7-devel-ubuntu18.04

%labels
  maintainer Miguel Carcamo <miguel.carcamo@postgrad.manchester.ac.uk>
  package.name
  package.version 1.0
  package.homepage
  package.source.url
  package.source.mdm5
  package.license GPLv3
%environment
    SHELL=/bin/bash
    PATH=/usr/local/cuda-10.1/bin${PATH:+:${PATH}}
    LD_LIBRARY_PATH=/usr/local/cuda-10.1/lib64${LD_LIBRARY_PATH:+:${LD_LIBRARY_PATH}}

%post
    apt -y man
    apt -y vim
    apt -y autoconf
    apt -y libtool
    apt -y automake
    apt -y install libboost-all-dev
    apt -y install apt-utils
    apt -y install software-properties-common
    apt -y install udev
    add-apt-repository universe
    apt update
    apt -y install python2.7
    apt -y install python-pip
    apt -y install python3.6
    apt -y install python3-pip
    apt -y install python-tk
    apt -y install git
    pip3 install numpy
    pip3 install matplotlib
    pip3 install cython
    pip3 install pyfits
    pip3 install pywcs
    pip3 install astropy
    pip3 install pywt
    apt -y install curl
    apt -y install cuda
    apt -y install cmake
    apt -y install gfortran
    apt -y install g++
    apt -y install libncurses5-dev
    apt -y install libreadline-dev
    apt -y install flex
    apt -y install bison
    apt -y install libblas-dev
    apt -y install liblapacke-dev
    apt -y install libcfitsio-dev
    apt -y install wcslib-dev
    apt -y install libhdf5-serial-dev
    apt -y install libfftw3-dev
    apt -y install python-numpy
    apt -y install libboost-python-dev
    apt -y install libpython3.4-dev
    apt -y install libpython2.7-dev
%runscript
   
