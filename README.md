WPS-Office-Font-Installation

WPS' prebuild font package does not seem to install their fonts
properly, so I hope this will help others!

This script will move the folder 'special-wps-office-fonts' from the

downloaded/cloned folder to your system fonts folder.
On the other hand, this is my VERY FIRST attempt a making my own bash
script, so it might just be easier to install the fonts yourself by
following these instructions:

1a) Clone this repo somewhere and open the folder 1b) Download and
extract the .zip GitHub automatically makes. Then open that folder. 2)
Move or Copy the folder '`special-wps-office-fonts`' to
`/usr/share/fonts/` 3) Update your font-cache by entering these commands
based on your distrobution: a) I think that you can also probably just
use `sudo fc-cashe` for every distro, but here's instructions for
specific ones that I found online. a) Mint/Ubuntu/Debian/etc Distros:
`sudo fc-cache -f -v` b) Arch/Manjaro/Antergos/etc Distros:
`sudo fc-cache` c) Fedora/OpenMandriva/Mageia/etc Distros:
`sudo fc-cache -s` d) Misc Others: `sudo fc-cache`

You can also copy and paste this command into your terminal. First `cd`
to wherever your downloaded or cloned this folder. Then type this
depending on your distro:

Mint/Ubuntu/Debian/etc
`sudo mv -rf special-wps-office-fonts/ /usr/share/fonts/ ; sudo fc-cache -f -v ; cd`

Arch/Manjaro/Antergos/etc 
`sudo mv -rf special-wps-office-fonts/ /usr/share/fonts/ ; sudo fc-cache ; cd\`

Fedora/OpenMandriva/Mageia/etc
`sudo mv -rf special-wps-office-fonts/ /usr/share/fonts/ ; sudo fc-cache -s ; cd`

Other Distros
`sudo mv -rf special-wps-office-fonts/ /usr/share/fonts/ ; sudo fc-cache ; cd`

### 

You're done! WPS Office should now load properly! Awesome!

⁓ Ev


PS ⁓ Ev I'm sorry about the formatting of this  README.md,  it looks perfectly fine in my editor.  No idea why it looks so shitty here.
