# ZNY-Minero
Guia para minar ZNY-Linux

Seguir todos los pasos de abajo con el terminal

- Actualizar

Sudo apt-get update

sudo apt install git curl unzip gedit automake autoconf dh-autoreconf build-essential pkg-config openssh-server screen libtool libcurl4-openssl-dev libtool libncurses5-dev libudev-dev


- Build

cd ~

git clone https://github.com/BitzenyCoreDevelopers/cpuminer.git

cd ~/cpuminer

chmod +x autogen.sh

./autogen.sh

./configure CFLAGS="-O3 -march=native"

make

sudo make install

- Minar

cd ~/cpuminer

./minerd -a yescrypt -o stratum+tcp://wpool.work:15020 -u DIRECCION-WALLET



Donaciones - ZmeV1zapwaLBBJ3nuXHYBoYqaeLjXtmS5v
