My build of dwm 6.2 with custom patches (and keybindings, in `config.h`). See [https://dwm.suckless.org/](https://dwm.suckless.org/) for details on the dwm window manager, how to build and install it, and how it works.

---

- alternativetags
      - Introduces alternative tag labels that can be switched on or off on the fly
      - Keybindings included in `config.h`
      - Refer to [https://dwm.suckless.org/patches/alternativetags/](https://dwm.suckless.org/patches/alternativetags/)



- gaplessgrid
      - From the patch's description:
     > This patch is an altered gridmode layout for dwm, which arranges the windows in a grid. Instead of using a regular grid, which might leave empty cells when there are not enough windows to fill the grid, it adjusts the number of windows in the first few columns to avoid empty cells.
      
      - Refer to [https://dwm.suckless.org/patches/gaplessgrid/](https://dwm.suckless.org/patches/gaplessgrid/)



This patch is an altered gridmode layout for dwm, which arranges the windows in a grid. Instead of using a regular grid, which might leave empty cells when there are not enough windows to fill the grid, it adjusts the number of windows in the first few columns to avoid empty cells.

- pertag
      - The pertag patch keeps layout, mwfact, barpos and nmaster settings per tag, rather than the default behaviour of having everything global across all tags
      - I borrowed the configurable nature of pertag and the patch for dwm 6.2 from [https://github.com/bakkeby/dwm-vanitygaps](bakkeby's dwm build)
      - Refer to [https://dwm.suckless.org/patches/pertag/](https://dwm.suckless.org/patches/pertag/)
