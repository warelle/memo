

make distclean
rm config.cache
./configure --target=gaia-elf --prefix=/home/shohei/gaia-test/
make all

gcc/contrib/download_prerequisites
../configure target=m32r-unknown-linux --enable-multilib --with-system-zlib


./configure --target=aqua-elf --prefix=/home/shohei/aqua
make -j4
make install
export PATH=$PATH:/home/shohei/aqua/bin
./configure --target=aqua-elf --prefix=/home/shohei/aqua
make -j4
make install
