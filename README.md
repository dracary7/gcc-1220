编译gcc命令

```shell
make distclean && make clean
find -name "config.cache" -print0 | xargs -0 rm
./contrib/download_prerequisites
./configure --prefix=/mnt/sda1/lxw/syzbot-0ca89728/gccbuild1 -enable-checking=release -enable-languages=c,c++ --disable-multilib
```
