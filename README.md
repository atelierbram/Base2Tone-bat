# Base2Tone bat
Dark duotone colorschemes for [bat](https://github.com/sharkdp/bat); a cat(1) clone with wings. These colorschemes are based on [DuoTone themes](https://simurai.com/projects/2016/01/01/duotone-themes) by [Simurai](https://simurai.com/). For light variations take the ones on [github.com/atelierbram/Base2Tone-Sublime-Text](https://github.com/atelierbram/Base2Tone-Sublime-Text).

## Adding themes
Create a folder for the new syntax highlighting themes, clone this repo over there:
```bash
mkdir -p "$(bat --config-dir)/themes"
cd "$(bat --config-dir)/themes"
git clone https://github.com/atelierbram/Base2Tone-bat
```
## Update the binary cache
```bash
bat cache --build
```

Finally, use `bat --list-themes` to check if the new themes are available, or just try it out in the terminal:

```bash
bat --theme=base2tone-evening-dark README.md
```

To set a theme more permanently a default configuration file can be created with the `--generate-config-file` option.

```bash
bat --generate-config-file
```

You can set one of the themes over there in `~/.config/bat/config` like:

```bash
--theme="base2tone-evening-dark"
```

or put it in a `.bashrc` or `.zshrc` configuration file:

```bash
export BAT_THEME="base2tone-evening-dark"
```

## Base2Tone
- [Base2Tone on Github](https://github.com/atelierbram/Base2Tone)
- [Base2Tone demo site](https://base2t.one/)

## Credits
- Credits to [Simurai](https://simurai.com/) whose [DuoTone themes](https://simurai.com/projects/2016/01/01/duotone-themes) for Atom were a model for these colorschemes

### Resources
- [Orginal Colorscheme for Atom on simurai.com](https://simurai.com/projects/2016/01/01/duotone-themes)
- [Orginal Colorscheme for Atom on Github](https://github.com/simurai/duotone-dark-syntax/)

## License
Released under [MIT Licence](https://atelierbram.mit-license.org)
