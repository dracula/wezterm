### [WezTerm](https://wezfurlong.org/wezterm)

#### Install using Git

If you are a git user, you can install the theme and keep up to date by cloning the repo:

    git clone https://github.com/dracula/wezterm.git

#### Install manually

Download using the [GitHub .zip download](https://github.com/dracula/wezterm/archive/master.zip) option and unzip it.

#### Activating theme

1. Copy paste `dracula.lua` to WezTerm's directory
2. Edit your `wezterm.lua` file under WezTerm's directory with the following content:

```lua
local dracula = require 'dracula';
return {
    colors = dracula,
    tab_bar_at_bottom = true,
    use_fancy_tab_bar = false
}
```

The location of WezTerm's directory varies between platforms:

-   \*nix: `$HOME/.config/wezterm/`
-   Windows: directory that contains `wezterm.exe`

#### Alternative

Use the dracula theme bundled with WezTerm (uses iTerm2 colors, and without tab bar stylings)

Edit your `wezterm.lua` file under WezTerm's directory with the following content:

```lua
return {
	color_scheme = "Dracula"
}
```
