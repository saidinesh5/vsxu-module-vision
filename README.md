vsxu sample module
==================

Sample Module For VSXu.

All it does is take 2 float params for input and outputs a result = sum(inputs)

Installation:
---


Install the dependencies (Also make sure you already have a copy of libvsxu-dev installed):

    sudo apt-get install libopencv-dev libcvaux-dev libhighgui-dev libcv-dev

Now Compile and install the module:
    
    git clone git://github.com/vovoid/vsxu-module.git
    cd vsxu-module-vision
    mkdir build
    cd build
    cmake ..
    make
    make install

This automatically installs the plugin to the vsxu plugins directory.

You may need to run the "make install" command with administrator privileges.

However, if you have compiled vsxu locally (which is a better option), 
you might want to set PKG_CONFIG_PATH to override the installed vsxu in
/usr/lib/vsxu

Add this to your ~/.bash_aliases (or your other favourite bash startup script):

    export PKG_CONFIG_PATH='/path/to/install/lib/pkgconfig'

This will make cmake find the VSXu installation in the correct directory.
