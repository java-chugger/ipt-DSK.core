#!/human.mk-1

# $script_rootdir/README.txt
# miphix@insomnia247.nl
# 26 July, 2017

This collection of scripts is intended for a Debian compatible Linux system to
provide an iptables script that is prevelant from boot to boot without clunky
tools as iptables-persistent. You will find an amalgamation of scripts that have
been drawn from BoneKrackers examples on ipset to compliment my iptables and
friends scripts. You will have to do some homework on mapping your own local
broadcast domain (partaining to the targetted systems con-joined network.). to
benefit from the series of scripts here in. i.e., '**/99-static_arp.sh'. 

As of this moment, I have yet to have written a 'make' style file to populate
the intended directories with the referenced files. Naturally, I intend to put
this together in due time. However, since I have yet to do that, if you're
reading this, you will have to locate the target directory and file name in the
files header. This is indicated in the format as:

#!/bin/bash --

# /usr/local/bin/arrdvarks_resolve.ext

Where /usr/local/bin/ is the intended directory for the script to be placed. and
arrdvarks_resolve.ext is the file being currently read. 

This repository will contain:

  - an initialization script for the core iptables script.
    - the aforementioned core iptables script
      - chain specific scripts targetted at protocols
  - IPSet scripts (not all of them are authored by me: kudos BoneKracker, nice
    work!)
  - a static arp script ( -REVIEW AND REVISE FOR ==YOUR== ENVIRONMENT- )
