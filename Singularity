Bootstrap: shub
From: sujoyp/cuda-9.0-base-simu

%post

    # OGRE
    git clone https://github.com/sujoyp/ogre.git
    cd ogre/sinbad-ogre-4c20a40dae61/
    mkdir build
    cd build
    cmake -DFREETYPE_INCLUDE_DIR=/usr/include/freetype2 \
    -DFREETYPE_FT2BUILD_INCLUDE_DIR=/usr/include/freetype2 \
    -DOGRE_CONFIG_THREADS=0 \
    ..
    make -j8
    cmake -DCMAKE_INSTALL_PREFIX=/usr/local/OGRE .
    make install
    
