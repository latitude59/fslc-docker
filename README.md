# fslc-docker

```
$ repo init -u git@github.com:latitude59/fslc-docker.git -m default.xml -b master
$ repo sync -j4
$ MACHINE=imx7d-pico DISTRO=fslc-framebuffer . setup-environment build
$ ln -s ~/yocto_downloads ../downloads
$ time bitbake core-image-minimal
```
