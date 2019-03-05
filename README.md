# local_manifests
For sony rhine platform


    mkdir xosp
    cd xosp
    
    repo init -u git://github.com/XOSP-Project/platform_manifest.git -b xosp-n-rebase
    
    mkdir local_manifests
    
    curl https://raw.githubusercontent.com/raschad/local_manifests/xosp-n/roomservice.xml > ~/xosp/.repo/local_manifests/roomsrvice.xml
