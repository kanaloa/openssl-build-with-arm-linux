# openssl-build-with-arm-linux

* wget https://www.openssl.org/source/openssl-1.0.2f.tar.gz
* tar xzvf openssl-1.0.2f.tar.gz
* cd openssl-1.0.2f
* ./Configure linux-generic32 shared -DL_ENDIAN --prefix=/tmp/openssl --openssldir=/tmp/openssl
* make install CC=arm-linux-gcc RANLIB=arm-linux-ranlib LD=arm-linux-ld MAKEDEPPROG=arm-linux-gcc PROCESSOR=ARM
