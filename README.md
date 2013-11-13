# i3-style

Make your [i3](http://i3wm.org) config a little more stylish.

**Warning:** i3-style is experimental. It may eat your config! Please back up your config file every time you use it until it is stable.

## About

i3-style applies a theme to your i3 config file to change the colorscheme of the window decorations and the different parts of i3bar. It's designed especially for people who make frequent changes to their colorscheme to get things just right.

* Easy to try out new themes right after you install.
* Themes are easy to read, modify, and share.
* Modifies your theme in place - extra template files are not needed.

For an overview of the capabilities of i3-style, see my [blog post](http://dubstepdish.com/blog/2013/11/06/introducing-i3-style/).

## Installing

To install with [npm](https://npmjs.org/):

    npm install -g i3-style

The `i3-style` executable should now be in your PATH.

## Usage

First of all, it's always a good idea to make a backup of your config before you try a new theme so you can get things back to how they were. Then just call `i3-style` with the name of the theme you want to try and where you want to write the config file to. i3-style will look for your config in the default place and apply the theme. Then just reload and enjoy the new theme.

    cp ~/.i3/config ~/.i3/config.backup
    i3-style solarized -o ~/.i3/config
    i3-msg reload

Check the `themes` directory for the list of built-in themes.

If you want to modify a theme, copy it from `themes` and give it a `.yaml` extension. The object format is [well-documented](https://github.com/acrisci/i3-style/blob/master/doc/spec.md) and includes support for color aliases. Then back up your config and call i3-style.

    i3-style ~/.i3/solarized.yaml -o ~/.i3/config

Just keep doing that until you get it perfect (which might be never).

## Contributing - Send us themes!

If you've made a new theme, or made an improvement to an existing theme, please make a pull request adding your theme to the `themes` directory!

## License

This work is available under a FreeBSD License (see LICENSE).

Copyright © 2013, Tony Crisci

All rights reserved.
