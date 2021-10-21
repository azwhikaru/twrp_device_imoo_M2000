imoo C1
===============
```
By : Aizawa Hikaru
```

![Picture](https://s9.rr.itc.cn/r/wapChange/201612_24_2/a494zm7286571603855.jpg)

This is a Minimal Device Tree for building TWRP for imoo C1 (Codename: M2000). 

Basic        | Spec Sheet
------------:|:------------------------
CPU          | Cortex-A53 Eight-Core MT6755 (Heilo P10)
Memory       | 3GB RAM
Shipped Android Version | 6.0
Storage      | 32GB eMMC5.1
Display      | 5.5

This branch is for building TWRP.

### Thanks to:
 * Myself

### To build: 

```
$ mkdir twrp

$ cd twrp

$ repo init -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-6.0

To initialize a shallow clone, which will save even more space, use a command like this:

$ repo init --depth=1 -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_omni.git -b twrp-6.0

After that sync your sources:

$ repo sync

Download or clone this repository, go to /twrp/device and create imoo/M2000. Copy this repo to your created folder

Build your recovery:

$ source build/envsetup.sh

& lunch omni_M2000

make clean && make recoveryimage
```
