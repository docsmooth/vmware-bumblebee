vmware-bumblebee
================

Bash Script to start VMware Workstation under Bumblebee Primus/Optimus hybrid drivers

Information and history on this blog post: http://www.totalnetsolutions.net/2012/12/08/bumblebee-primus-and-vmware-workstation-nvidia-optimus-graphics-on-ubuntu/


To new users, especially those coming from other forum posts: Please check the issues tab.  I only have Ubuntu, but other developers have added Fedora, OpenSUSE, Arch, and Debian support.  I'm using the Issues to track things that aren't working, and as you can see, this is still actively developed, but it needs feedback for that to work.

Last Updated 2017-08-07

To use:
mkdir -p ~/bin
cd ~/bin

git clone https://github.com/docsmooth/vmware-bumblebee.git

OR

wget https://github.com/docsmooth/vmware-bumblebee/blob/master/vmware && ln -s ./vmware vmplayer

This will place the scripts as executable in your $HOME/bin, so they can be launched from anywhere.

For the first time, or after any update, run "sudo vmware -i" to install the helper.

To use normally, just run "vmware" or "vmplayer" and your default path SHOULD pick this up before the default VMware installed version in /usr/bin/vmware

There are flags "--no" and "--yes" to force disable/enable 3d.  If you're on battery, the script should NOT launch the 3d routines, and VMware might complain about a missing 3d compatible video card.  That's OK.

Thank you in advance for any help with bugs, issues, comments.

As of July, 2017, my primary laptop does NOT have an NVidia card, so I'm personally not using this daily anymore, but still have the hardware, it still runs 100% of the time, and I'm still active on this project.
