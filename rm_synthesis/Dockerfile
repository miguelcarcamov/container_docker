FROM ubuntu:18.04

ENV SHELL /bin/bash
ENV TZ=Europe/Minsk
ENV LD_LIBRARY_PATH /usr/lib:/usr/local/lib:$LD_LIBRARY_PATH
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
RUN echo "deb mirror://mirrors.ubuntu.com/mirrors.txt bionic main restricted universe multiverse" >> /etc/apt/sources.list
RUN echo "deb mirror://mirrors.ubuntu.com/mirrors.txt bionic-updates main restricted universe multiverse" >> /etc/apt/sources.list
RUN echo "deb mirror://mirrors.ubuntu.com/mirrors.txt bionic-security main restricted universe multiverse" >> /etc/apt/sources.list
RUN apt-get update && \
	apt-get -y install tzdata software-properties-common && \
	add-apt-repository main && add-apt-repository universe && add-apt-repository restricted && add-apt-repository multiverse && \
    apt-get update && \
    apt-get -y install apt-utils man vim autoconf libtool automake libboost-all-dev \
    	python3-pip python3-tk python-tk git && \
    pip3 install numpy && \
    pip3 install matplotlib && \
    pip3 install cython && \
    pip3 install pyfits && \
    pip3 install pywcs && \
    pip3 install astropy && \
    pip3 install PyWavelets && \
    pip3 install scipy && \
    pip3 install toolz && \
    pip3 install dask && \
    pip3 install mpi4py && \
    apt-get -y install curl cmake gfortran g++ libncurses5-dev libreadline-dev flex bison libblas-dev \
    	cmake liblapacke-dev libcfitsio-dev wcslib-dev libhdf5-serial-dev libfftw3-dev python-numpy \
	libboost-python-dev libpython3.6-dev libpython2.7-dev htop libcr-dev mpich mpich-doc saods9 && \
    git clone --single-branch --branch master https://github.com/miguelcarcamov/rm_synthesis_simple.git
