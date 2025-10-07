# Colorschemes for the Linux TTY

## Installation

- `./install` to install `tty-colorscheme` along with various themes.
- `./install remove` to uninstall it.

## Usage

```
tty-colorscheme [option] | [colorscheme]
  -l    List available colorschemes
  -f    List available PSF fonts
  -p    Print the current palette
  -c    Cycle through colorschemes and fonts
```

Changing colors across all TTYs requires `sudo`.

If you encounter screen artifacts, press `Ctrl+L` or type `clear`.

To revert to the system default colors, type `reset`.

To apply a colorscheme automatically upon login, add `tty-colorscheme [colorscheme]` to your `~/.profile`.

## Screenshots

### monokai-soda
![monokai-soda](images/monokai-soda.png)

### mono-amber
![mono-amber](images/mono-amber.png)

### mono-light
![mono-light](images/mono-light.png)

### blood-dragon
![blood-dragon](images/blood-dragon.png)

## Customization

A colorscheme file has the following format:

```
color01="000000" # Black (Background)
color02="F44336" # Red
color03="4CAF50" # Green
color04="FFEB3B" # Yellow
color05="2196F3" # Blue
color06="9C27B0" # Magenta
color07="00BCD4" # Cyan
color08="9E9E9E" # White (Foreground)
color09="000000" # Black
color10="F44336" # Red
color11="4CAF50" # Green
color12="FFEB3B" # Yellow
color13="2196F3" # Blue
color14="9C27B0" # Magenta
color15="00BCD4" # Cyan
color16="9E9E9E" # White
```

To create a custom colorscheme, modify the HEX values and place the file in `/etc/tty-colorscheme/colorschemes`.
