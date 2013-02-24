rotorsync
=========

A simple system backup script using rsync written in bash.

This script is used to take system and configuration snapshots. It can maintain either a single snapshot or multiple incremental 
snapshots. Snapshots are split into 2 directories: "ROOT/" and "DOTFILES/". 
ROOT/: Stores snapshots of the root tree excluding /home/.
DOTFILES/: Stores snapshots of the users hidden files found in /home/username/ 
A sample of a service file is included for use with systemd. with sysvinit users can simply add the path to this script as a last
entry in /etc/rc.local.
to use simply copy this script into /usr/bin/ and mark as executable: chmod a+x /usr/bin/rotorsync.
#Unfinished Readme as of now... more  explanation later#
 
