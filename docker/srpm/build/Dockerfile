FROM fedora:21

MAINTAINER "Jiao Lin <jiao.lin@gmail.com>"

RUN yum install -y git cmake make gcc-c++ python python-devel rpm-build
RUN mkdir /danse.ins
WORKDIR /danse.ins
RUN git clone https://github.com/danse-inelastic/danse.ins
RUN mkdir build
WORKDIR /danse.ins/build
RUN cmake ../danse.ins
RUN make srpm
