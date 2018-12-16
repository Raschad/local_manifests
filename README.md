# local_manifests
For sony rhine platform
Usage
=====
    
Create folder

    mkdir dot

Then

    cd dot
    
initialize repo:

    repo init -u git://github.com/DotOS/manifest.git -b dot-n
    
sync repo:

    $ repo sync  -f --force-sync --no-clone-bundle
    

---------------
download manifest: 

    curl https://raw.githubusercontent.com/raschad/local_manifests/dot-n/roomservice.xml > ~/dot/.repo/local_manifests/roomservice.xml

sync repo:

    $ repo sync  -f -j16 --force-sync --no-clone-bundle

build DotOS
build:

    . build/envsetup.sh
    brunch honami
