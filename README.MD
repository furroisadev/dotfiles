# Furro's BSPWM Rice Guide

A minimal but sleek X11 rice using **bspwm**, **picom**, **polybar**, and **pywal** with a purple starry aesthetic. Designed to work without a display manager (no LightDM), and confirmed to work with AMD cards using the `amdgpu` driver.

---

## 🔧 Dependencies

Install the following packages:

```bash
sudo apt install bspwm sxhkd xorg xinit alacritty picom rofi polybar git curl unzip
```

Also install pywal with pipx (recommended)
```bash
pipx install pywal
```
Ensure pipx is set up in your shell
```bash
pipx ensurepath
```
Ensure you have the xinit package installed (assuming you aren't using a display manager eg. lightdm, gdm3, or sddm)

```bash
sudo apt install xinit
```
the start it with
```bash
startx
```

##Useful Notes

###Pywal not applying to new terminals?

Add this to your shell config (e.g. ~/.zshrc or ~/.bashrc)
```bash
[ -f "$HOME/.cache/wal/sequences" ] && cat "$HOME/.cache/wal/sequences"
```
