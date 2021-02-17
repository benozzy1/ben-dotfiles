# Ben Dotfiles 
My personal dotfiles for a custom bspwm linux setup. (USE AT YOUR OWN RISK!)

Dotfiles present in this repo:
  * bspwm
  * kitty
  * picom
  * sxhkd

# Instructions
Clone the repo:
```
git clone https://github.com/benozzy1/ben-dotfiles.git
cd ben-dotfiles
```

To link the config files, you first have to remove your currently existing ones (CREATE A BACKUP BEFORE YOU DO THIS!!!):
```
rm ~/.config/bspwm/bspwmrc
rm ~/.config/kitty/kitty.conf
rm ~/.config/picom/picom.conf
rm ~/.config/sxhkd/sxhkdrc
```

To make sure you have the config directories, create them:
```
mkdir ~/.config/bspwm
mkdir ~/.config/kitty
mkdir ~/.config/picom
mkdir ~/.config/sxhkd
```

Then, you have to create hard symlinks from each file in the repo to your .config folder (located in $HOME/.config):
```
ln ./.config/bspwm/bspwmrc ~/.config/bspwm/bspwmrc
ln ./.config/kitty/kitty.conf ~/.config/kitty/kitty.conf
ln ./.config/picom/picom.conf ~/.config/picom/picom.conf
ln ./.config/sxhkd/sxhkdrc ~/.config/sxhkd/sxhkdrc
```

Picom's default config is inside `~/.config/picom.conf` and my dotfiles have its config folder inside `~/.config/picom/picom.conf`. To change config for picom enter this command:
`picom --config ~/.config/picom/picom.conf`

And that's it! These config files were made by me for my own personal use, though you can choose to use them yourself at your own risk. Do note that I am not very experienced working with dotfiles and these are not guarenteed to work on your system.
