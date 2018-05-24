# minor fork of vim-gnupgp

James McCoy's GNU pgp plugin
https://github.com/jamessan/vim-gnupg

With my usability enhancements.

* documentation
* hide GPG* commands unless needed. The ":GXXX" commands in my workflow are all
  tpope/fugitive commands, and I'd rather not see the GPGXXX commands show in
  tab completion unless they are actually relevant.

The original plugin seems quite solid, but it looks to be in heavy maintenance
mode, with old "all in one file" style packaging (I'd expect pre path manager
approach). There are 2 pull requests for documentation that are 1-4 years old.

So... to scratch my itch, I've forked his plugin.

# Original Description

This script implements transparent editing of gpg encrypted files. The filename
must have a ".gpg", ".pgp" or ".asc" suffix. When opening such a file the
content is decrypted, when opening a new file the script will ask for the
recipients of the encrypted file. The file content will be encrypted to all
recipients before it is written. The script
http://www.vim.org/scripts/script.php

