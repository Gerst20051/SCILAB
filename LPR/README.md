# Steps To Install SIP (Scilab Image Processing Toolbox)

## Install Autoconf
[$]> curl -OL http://ftpmirror.gnu.org/autoconf/autoconf-2.69.tar.gz
[$]> tar -xzf autoconf-2.69.tar.gz
[$]> cd autoconf-2.69
[$]> ./configure && make && sudo make install

## Install Automake
[$]> curl -OL http://ftpmirror.gnu.org/automake/automake-1.14.tar.gz
[$]> tar -xzf automake-1.14.tar.gz
[$]> cd automake-1.14
[$]> ./configure && make && sudo make install

## Install Libtool
[$]> curl -OL http://ftpmirror.gnu.org/libtool/libtool-2.4.2.tar.gz
[$]> tar -xzf libtool-2.4.2.tar.gz
[$]> cd libtool-2.4.2
[$]> ./configure && make && sudo make install

## Download & Install MacPorts
https://www.macports.org/install.php

# Install Xcode Command Line Tools
[$]> xcode-select --install

## Install ImageMagick (Also Installs Autoconf, Automake, and Libtool)
[$]> sudo port install ImageMagick
   > dependencies to be installed: autoconf m4 perl5 perl5.16 gdbm gettext expat libiconv ncurses automake bzip2 djvulibre jpeg tiff xz zlib fftw-3 fontconfig freetype libpng ghostscript jbig2dec libidn libpaper libtool pkgconfig xorg-libXext xorg-libX11 xorg-kbproto xorg-libXau xorg-xproto xorg-libXdmcp xorg-libxcb python27 db48 db_select libedit openssl python_select sqlite3 xorg-libpthread-stubs xorg-xcb-proto libxml2 xorg-xextproto xorg-libXt xorg-libsm xorg-libice jbigkit lcms2 openexr ilmbase openjpeg urw-fonts webp

# Add Scilab & Animal To Your Environment PATH
[$]> vi ~/.bash_profile
   > export PATH=$PATH:/Applications/scilab-5.5.1.app/Contents/MacOS/bin/
   > export PATH=$PATH:~/web/git/scilab/animal/bin
   > export ANIMAL_CONFIG=~/web/git/scilab/animal/config
[$]> . ~/.bash_profile

# Run Install SIP
[$]> ./install-sip
