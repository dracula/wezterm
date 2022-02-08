### [WezTerm](https://wezfurlong.org/wezterm)

#### Installation

Edit your `wezterm.lua` file with the following content:

```lua
return {
    colors = {
        foreground = "#f8f8f2",
        background = "#282a36",
        cursor_bg = "#f8f8f2",
        cursor_fg = "#282a36",
        cursor_border = "#f8f8f2",
        selection_fg = "#282a36",
        selection_bg = "#44475a",
        scrollbar_thumb = "#44475a",
        split = "#bd93f9",
        ansi = {"#21222C", "#FF5555", "#50FA7B", "#F1FA8C", "#BD93F9", "#FF79C6", "#8BE9FD", "#F8F8F2"},
        brights = {"#6272A4", "#FF6E6E", "#69FF94", "#FFFFA5", "#D6ACFF", "#FF92DF", "#A4FFFF", "#FFFFFF"},
        indexed = {
            [136] = "#44475A"
        },
        compose_cursor = "#FFB86C",
        tab_bar = {
            background = "#282a36",
            active_tab = {
                bg_color = "#bd93f9",
                fg_color = "#282a36",
                intensity = "Normal",
                underline = "None",
                italic = false,
                strikethrough = false
            },
            inactive_tab = {
                bg_color = "#282a36",
                fg_color = "#f8f8f2"
            },
            inactive_tab_hover = {
                bg_color = "#6272a4",
                fg_color = "#f8f8f2",
                italic = true
            },
            new_tab = {
                bg_color = "#282a36",
                fg_color = "#f8f8f2"
            },
            new_tab_hover = {
                bg_color = "#ff79c6",
                fg_color = "#f8f8f2",
                italic = true
            }
        }
    },
    tab_bar_at_bottom = true,
    use_fancy_tab_bar = false
}
```

The location of the `wezterm.lua` varies between platforms:

-   \*nix: File defined as `$WEZTERM_CONFIG_FILE` or `$HOME/.config/wezterm/wezterm.lua` or `$HOME/.wezterm.lua`
-   Windows: directory that contains `wezterm.exe`
