gentoo-overlay
==============

This is my personal Gentoo Portage Overlay for my own usage.
An overlay is an additional repository for Portage. It contains
additional (modified) ebuilds for Gentoo.

Currently, my overlay contains:
### Dmenu with QXYW Patch and WM_CLASS Patch
Dmenu with some additional options: quiet, XY offset, and width.

**Update 2:** Add height patch (I got from [here](https://gist.github.com/runiq/1755434))

**Update 1:** Add WM_CLASS patch (I got from [here](https://bbs.archlinux.org/viewtopic.php?pid=563279))

I got the QXWY patch from [here](https://github.com/baskerville/dmenu_qxyw).


But, that patch doesn't support Xft. So, I modified ebuild from Portage
that has Xft patch. I merged both Xft and QXYW patch, created Xft-QXYW patch.
The **xft** USE Flag must be enabled to make QXYW feature works.
(I don't know how to add USE Flag)

### Dzen with Xft Support (Removed)
Dzen with Xft support has already in main Portage tree (dzen-0.9.5-r1) since 30 September 2013.
