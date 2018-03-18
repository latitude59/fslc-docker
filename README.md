# fslc-docker

```
$ repo init -u git@github.com:latitude59/fslc-docker.git -m default.xml -b master
$ repo sync -j4
```
Initial run:
```
$ TEMPLATECONF=../sources/meta-fslc-docker/conf/ . sources/poky/oe-init-build-env build/
```
Change `MACHINE` and `DISTRO` in `build/conf/local.conf` if required.

For subsequent runs:
```
. sources/poky/oe-init-build-env build/
```
Then:
```
$ ln -s ~/yocto_downloads/ ../downloads/
$ time bitbake core-image-minimal
```
