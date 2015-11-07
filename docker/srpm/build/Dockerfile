FROM linjiao/danse.ins-srpm-deps

MAINTAINER "Jiao Lin <jiao.lin@gmail.com>"

RUN mkdir /danse.ins
WORKDIR /danse.ins
RUN git clone https://github.com/danse-inelastic/danse.ins
RUN mkdir build
WORKDIR /danse.ins/build
RUN cmake ../danse.ins -DCMAKE_INSTALL_PREFIX=/opt/danse
RUN make srpm
