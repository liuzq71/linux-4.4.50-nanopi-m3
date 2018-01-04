It is forked from https://github.com/friendlyarm/linux.git -b nanopi2-v4.4.y
build:
   $touch .scmversion
   $make ARCH=arm64 nanopi3_linux_defconfig
   $make ARCH=arm64 CROSS_COMPILE=aarch64-linux-gnu- Image -j4
