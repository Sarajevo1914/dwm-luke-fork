# Fork of Luke's build of dwm

I tried to create my own build from scratch but I got tired of having so many errors after applying more than 3 patches, then I kept trying with dwm-flexipatch but for some reason I can't get it to work, I still have compilation errors and although I manage to correct them, modify the config.h is a pain in the ass, so the only thing I can think of is to modify an already made base, in this case Luke Smith's build, I know that Derek Tyler also has his own build but DTOS is a bit bloat, my machine literally explodes With so many resources and things in the background, I could try to use its build separately but there are two reasons why I didn't.
1. I want to experience the full DTOS experience and not just a small part
2. I'm a lazy wanker


## Patches and features (from original luke)

- [Clickable statusbar](https://dwm.suckless.org/patches/statuscmd/) with my build of [dwmblocks](https://github.com/lukesmithxyz/dwmblocks).
- Reads [xresources](https://dwm.suckless.org/patches/xresources/) colors/variables (i.e. works with `pywal`, etc.).
- scratchpad: Accessible with <kbd>mod+shift+enter</kbd>.
- New layouts: bstack, fibonacci, deck, centered master and more. All bound to keys <kbd>super+(shift+)t/y/u/i</kbd>.
- True fullscreen (<kbd>super+f</kbd>) and prevents focus shifting.
- Windows can be made sticky (<kbd>super+s</kbd>).
- [hide vacant tags](https://dwm.suckless.org/patches/hide_vacant_tags/) hides tags with no windows.
- [stacker](https://dwm.suckless.org/patches/stacker/): Move windows up the stack manually (<kbd>super-K/J</kbd>).
- [shiftview](https://dwm.suckless.org/patches/nextprev/): Cycle through tags (<kbd>super+g/;</kbd>).
- [vanitygaps](https://dwm.suckless.org/patches/vanitygaps/): Gaps allowed across all layouts.
- [swallow patch](https://dwm.suckless.org/patches/swallow/): if a program run from a terminal would make it inoperable, it temporarily takes its place to save space.

## Change made by me

- unpatch hide tags (parcial, now show all tags but still dosents draw?)
- pertag
- change keybidings to my taste
- delete alot of stuff i dont use (aka bloat)

## Installation for newbs

```bash
git clone https://github.com/Sarajevo1914/dwm-luke-fork.git
cd dwm-luke-fork
sudo make install
```

There is also a `PKGBUILD` usable on distributions with pacman. Run `makepkg -si` instead of `sudo make install`.
