This is my personal ublock origin filter list.

This list removes a bunch of annoyances such as cookie warnings, reminders to
use the mobile app, and adblock shaming.

USE: Add this URL as a custom filter list in uBlock Origin
https://raw.githubusercontent.com/rberg2/rblock-list/master/rblock-filters.txt

BEWARE: I have a high tolerance for breakage, the alternative is that I will
not use some of these sites without adblock

Note to self: I used this command to sort the list, found here : https://stackoverflow.com/questions/11315889/how-to-sort-with-multiple-lines-in-bash

sed -r ':r;/(^|\n)$/!{$!{N;br}};s/\n/\v/g' rblock-filters.txt | sort | sed 's/\v/\n/g' >rblock-filters1.txt
