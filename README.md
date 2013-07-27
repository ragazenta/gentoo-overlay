gentoo-overlay
==============

This is my personal Gentoo Portage Overlay for my own usage.
An overlay is an additional repository for Portage. It contains
additional (modified) ebuilds for Gentoo.

Currently, my overlay contains:
### Dmenu with QXYW Patch
Dmenu with some additional options: quiet, XY offset, and width.
I got the QXWY patch from [here](https://github.com/baskerville/dmenu_qxyw).
But, that patch doesn't support Xft. So, I modified ebuild from Portage
that has Xft patch. I merged both Xft and QXYW patch, created Xft-QXYW patch.
The **xft** USE Flag must be enabled to make QXYW feature works.
(I don't know how to add USE Flag)

### Dzen with Xft Support
Dzen with Xft support. Actually, it has already in main Portage tree
as unstable package (dzen-0.9.5) since 18 July 2013.
I got the ebuild from [here](https://github.com/ojima-h/my-overlays).
