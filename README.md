My build of dwm 6.2 with custom patches (and keybindings, in `config.h`). See [https://dwm.suckless.org/](https://dwm.suckless.org/) for details on the dwm window manager, how to build and install it, and how it works.

To build dwm, on Debian 10 ("buster"), install the correct dependencies:

	sudo apt-get install make gcc libx11-dev libxft-dev libxinerama-dev libxrandr-dev

To actually use the X-server and the custom copy/paste commands, you'll have to install X.org as well:

	sudo apt-get install xorg xclip xvkbd
---

Patches included:

   - alternativetags
      - Introduces alternative tag labels that can be switched on or off on the fly
      - Keybindings included in `config.h`
      - Refer to [https://dwm.suckless.org/patches/alternativetags/](https://dwm.suckless.org/patches/alternativetags/)


   - gaplessgrid
      - From the patch's description:
     > This patch is an altered gridmode layout for dwm, which arranges the windows in a grid. Instead of using a regular grid, which might leave empty cells when there are not enough windows to fill the grid, it adjusts the number of windows in the first few columns to avoid empty cells.

      - Refer to [https://dwm.suckless.org/patches/gaplessgrid/](https://dwm.suckless.org/patches/gaplessgrid/)


   - monocle count
      - In contrast to the default behavior, this patch prints the total number of clients and the number of the currently activated client beside the symbol of the monocle layout instead of printing only the total number of clients
      - Refer to [https://dwm.suckless.org/patches/monocle_count/](https://dwm.suckless.org/patches/monocle_count/)


   - movestack
      - Allows you to move clients around in the stack and swap them with the master
      - Keybindings included in `config.h`
      - Refer to [https://dwm.suckless.org/patches/movestack/](https://dwm.suckless.org/patches/movestack/)


   - pertag
      - The pertag patch keeps layout, mwfact, barpos and nmaster settings per tag, rather than the default behaviour of having everything global across all tags
      - I borrowed the configurable nature of pertag and the patch for dwm 6.2 from [bakkeby's dwm build](https://github.com/bakkeby/dwm-vanitygaps)
      - Refer to [https://dwm.suckless.org/patches/pertag/](https://dwm.suckless.org/patches/pertag/)


   - status2d
      - Allows colors (and 2D rectangles) in the status bar
      - For color examples, see my [status bar script](https://github.com/aaronkirkman/statusbar)
      - To use colors: `^c#FF0000^` sets the foreground color and `^d^` resets the color to SchemeNorm
      - Refer to [https://dwm.suckless.org/patches/status2d/](https://dwm.suckless.org/patches/status2d/)
