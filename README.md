## STEPS_TO_BE_FOLLOWED_YOCTO_SETUP
Steps to bring up the setup


Installation of Dependent Libraries 


## Yocto Dependencies :

The following list shows the required packages by function given a supported Ubuntu or Debian Linux distribution
  ## sudo apt-get build-dep qemu 
  ## sudo apt-get remove oss4-dev
Essentials : Packages needed to build an image on a headless system: 
    
   ## sudo apt-get install gawk wget git-core diffstat unzip texinfo gcc-multilib build-essential chrpath socat cpio python python3 python3-pip python3-pexpect  xz-utils debianutils iputils-ping python3-git python3-jinja2 libegl1-mesa libsdl1.2-dev xterm
Documentation : Packages needed if you are going to build out the Yocto Project documentation manuals: 
   ## sudo apt-get install make xsltproc docbook-utils fop dblatex xmlto

## Legato Dependencies :

Legato Open Source Project is an initiative by Sierra Wireless Inc. which provides an open, secure and easy to use Application Framework for embedded devices.   

Prerequisites :
## sudo apt-get install -y autoconf automake bash bc bison bsdiff build-essential chrpath \ cmake cpio diffstat flex gawk gcovr git gperf iputils-ping libbz2-dev libcurl4-gnutls-dev \ libncurses5-dev libncursesw5-dev libsdl-dev libssl-dev libtool libxml2-utils ninja-build \ python python-git python-jinja2 python-pkg-resources python3 texinfo unzip wget zlib1g-dev

## Optional packages : openjdk-8-jdk (for Java support, at least Java 8 is required), doxygen graphviz (for doc generation), xsltproc (for running tests)
Cross-build toolchain(s)
For Sierra Wireless platforms, toolchains are available at 
https://source.sierrawireless.com/
Note : Toolchain of respective module to be used for development should be downloaded .

Once the above Dependencies are installed compile the source code using below command

## ==> make image_bin

flash the firmware located in 
Yocto-source/yocto/build_bin/tmp/deploy/images/swi-mdm9x28-wp/yocto_wp76xx.4k.cwe

One can use **swiflash** or **fwupdate** (via secure copy) to Update the firmware

