WPS-Office-Font-Installation

I downloaded wps-office_11.1.0.11691.XA_amd64.deb from wps-office official website. After installation I kept getting the "some formula symbols might not be displayed correctly due to missing fonts symbol"

WPS' prebuild font package does not seem to install their fonts
properly, so I hope this will help others!

This set of command lines would move the downloaded/cloned fonts to your system's WPS font folder.

1a) Clone this repo somewhere and open the folder 
1b) Download and extract the .zip GitHub automatically makes. Then open that folder. 

2) Move or Copy the folder's content to
`/usr/share/fonts/` 

3) Update your font-cache by entering the commands below
based on your distrobution: using ==> sudo fc-cache

You can also copy and paste this command into your terminal. First `cd`
to wherever your downloaded or cloned this folder. Then type this
depending on your distro:

Mint/Ubuntu/Debian/etc
`sudo mv -f *.* /usr/share/fonts/ ; sudo fc-cache -f -v ; cd`

Arch/Manjaro/Antergos/etc 
`sudo mv -f *.* /usr/share/fonts/  ; sudo fc-cache ; cd\`

Fedora/OpenMandriva/Mageia/etc
`sudo mv -f *.* /usr/share/fonts/ ; sudo fc-cache -s ; cd`

Other Distros
`sudo mv -f *.* /usr/share/fonts/  ; sudo fc-cache ; cd`

### 

You're done! WPS Office should now load properly! Awesome!

⁓ Ev


PS ⁓ Ev I'm sorry about the formatting of this  README.md,  it looks perfectly fine in my editor.  No idea why it looks so shitty here.
