ShirayukiProject
====================

How to Build?
-------------

To initialize your local repository, use a 
command like this:

```bash
repo init -u https://github.com/shirayuki-prjkt/yuki_manifest.git -b tsushima-13
```
  
Then to sync up:
----------------

```bash
repo sync -c --force-sync --no-tags --no-clone-bundle -j$(nproc --all) --optimized-fetch --prune
```

Setting up build environment:
----------------

```bash
. build/envsetup.sh
```

Lunch:
----------------

```bash
lunch shirayuki_<device_name>-userdebug
```

Build it:
----------------

```bash
mka shirayuki
```
