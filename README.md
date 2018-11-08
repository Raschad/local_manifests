# local_manifests
For sony rhine platform

Usage
=====
navigate into desired directory

initialize repo:

    repo init -u https://github.com/ResurrectionRemix/platform_manifest.git -b oreo

build RR (Oreo)
---------------
download manifest: 

    curl https://raw.githubusercontent.com/raschad/local_manifests/RR_o8.1/roomservice.xml > /your_directory/.repo/local_manifests/roomservice.xml

sync repo:

    $ repo sync -f --force-sync --no-clone-bundle

build:

    . build/envsetup.sh
    brunch honami
