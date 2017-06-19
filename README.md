Create omnirom directory to load sources:
```bash
mkdir ~/omnirom
cd ~/omnirom
repo init -u git://github.com/omnirom/android.git -b android-7.1'
```

Then use the following commands to load local_manifests for omnirom:

```bash
cd .repo
git clone https://github.com/xperia-aosp-project/local_manifests
cd local_manifests
git checkout omnirom
cd ../..
```

Then sync tour sources using

```bash
repo sync
```

Build rom like any other aosp rom using:

```bash
source build/envsetup.sh
brunch <device_name>
```