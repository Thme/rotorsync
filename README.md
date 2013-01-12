rotorsync
=========

A simple system backup script using rsync written in bash.

This script is used to take system and configuration snapshots. It can maintain either a single snapshot or multiple incremental 
snapshots. Snapshots are split into 2 directories: "ROOT/" and "DOTFILES/". 
ROOT/: Stores snapshots of the root tree excluding /home/.
DOTFILES/: Stores snapshots of the users hidden files found in /home/username/ 
