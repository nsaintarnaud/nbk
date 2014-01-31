nbk
===

A shell script that creates a backup of a file with the modification date in the filename:
filename.YYYYMMDD.hhmm.bak

Useful for taking snapshots of config files, /etc files, etc.

Works under *nix and OSX.  Accepts wildcards.

Example:
        $ ls -laF config
        -rw-r--r--   1 nsa  staff   572 Sep 21  2011 config
        $ nbk config
        $ ls -laF config*
        -rw-r--r--   1 nsa  staff   572 Sep 21  2011 config
        -rw-r--r--   1 nsa  staff   572 Sep 21  2011 config.20110921.1853.bak

