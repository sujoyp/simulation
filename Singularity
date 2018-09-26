Bootstrap: shub
From: sujoyp/cuda-9.0-base-simu

%post

    % OGRE
    mkdir workspace
    cd workspace
    mkdir 3rd_party
    cd 3rd_party
    mkdir -p ogre
    cd ogre
    wget https://bitbucket.org/sinbad/ogre/get/v1-9-0RC2.tar.gz
    tar zxf v1-9-0RC2.tar.gz
    cd sinbad-ogre-4c20a40dae61/
    mkdir build
    cd build
    cmake -DFREETYPE_INCLUDE_DIR=/usr/include/freetype2 \
    -DFREETYPE_FT2BUILD_INCLUDE_DIR=/usr/include/freetype2 \
    -DOGRE_CONFIG_THREADS=0 \
    ..
    make -j8
    cmake -DCMAKE_INSTALL_PREFIX=/usr/local/OGRE .
    make install
    
