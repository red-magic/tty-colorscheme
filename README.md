# Colorschemes for the linux TTY

## Installation

Run ```./install``` script as root to install ```tty-colorscheme``` and various themes.

```./install remove``` if you want to uninstall it.

## Usage

```
Usage: tty-colorscheme [-lpcrh | colorscheme]
  -l    list colorschemes
  -c    print current palette
  -r    set a random colorscheme
  -s    shift through colorschemes
  -h    print help
```

To change colors for a current TTY at user log on add ```tty-colorscheme [colorscheme]``` to ```.profile```.

It still requires using ```sudo``` if you want to change colors across all TTYs.

If you get screen artifacts hit ```Ctrl+l``` or type ```clear```.

Type ```reset``` to get back to the system default colors.

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

A colorscheme file looks like this:

```
color1=000000  # Black (Background)
color2=F44336  # Red
color3=4CAF50  # Green
color4=FFEB3B  # Yellow
color5=2196F3  # Blue
color6=9C27B0  # Magenta
color7=00BCD4  # Cyan
color8=9E9E9E  # White (Foreground)
color9=000000  # Black
color10=F44336 # Red
color11=4CAF50 # Green
color12=FFEB3B # Yellow
color13=2196F3 # Blue
color14=9C27B0 # Magenta
color15=00BCD4 # Cyan
color16=9E9E9E # White
```

Just change the hex values of colors and put it in ```/etc/tty-colorscheme/colorschemes``` directory.
