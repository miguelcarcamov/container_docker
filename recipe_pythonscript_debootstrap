BootStrap: debootstrap
OSVersion: bionic
MirrorURL: http://uk.archive.ubuntu.com/ubuntu/

%labels
  maintainer Miguel Carcamo <miguel.carcamo@postgrad.manchester.ac.uk>
  package.name
  package.version 1.0
  package.homepage
  package.source.url
  package.source.mdm5
  package.license GPLv3
%post
    apt update
    apt -y install build-essential
    apt install -y software-properties-common
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
    apt -y install curl
    curl -O https://developer.download.nvidia.com/compute/cuda/repos/ubuntu1804/x86_64/cuda-repo-ubuntu1804_10.1.105-1_amd64.deb
    dpkg -i cuda-repo-ubuntu1804_10.1.105-1_amd64.deb
    apt-key adv --fetch-keys https://developer.download.nvidia.com/compute/cuda/repos/ubuntu1804/x86_64/7fa2af80.pub
    apt update
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
   
