# AOSP EXTENDED NOUGAT for Xperia Z1(Honami)
For sony rhine platform

To initialize your local repository using the AospExtended trees, use a command like this:

    mkdir aosp
    cd aosp
    repo init -u git://github.com/AospExtended/manifest.git -b 7.x
create local_manifests

    mkdir .repo/local_manifests
    
    curl https://raw.githubusercontent.com/raschad/local_manifests/aex-n/roomservice.xml > ~/aosp/.repo/local_manifests/roomsrvice.xml
Then to sync up:

    repo sync -c -j32 --force-sync --no-clone-bundle --no-tags    
Finally to build:

    . build/envsetup.sh
    lunch aosp_device_codename-userdebug
    mka aex -jx
