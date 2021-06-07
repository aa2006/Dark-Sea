# `themer`

Your theme's unique URL:

https://themer.dev/?activeColorSet=dark&colors.dark.shade7=%23d1fffd&colors.dark.shade0=%230e2941&colors.dark.accent0=%23ff5877&colors.dark.accent1=%23296489&colors.dark.accent3=%2343c2da&colors.dark.accent2=%23b58ddb&colors.dark.accent4=%2366fcf1&colors.dark.accent5=%23d1e8e2&colors.dark.accent6=%23189cb4&colors.dark.accent7=%232e9cca&colors.dark.shade6=%23dedede&colors.light.shade0=%23e4fbff&colors.light.shade7=%23000946&colors.light.accent0=%23ff5877&colors.light.accent1=%2354b3bf&colors.light.accent2=%23b889c8&colors.light.accent3=%2300d8ff&colors.light.accent4=%233134f0&colors.light.accent5=%230006a1&colors.light.accent6=%235e00ff&colors.light.accent7=%232e9cca&calculateIntermediaryShades.dark=true

If you find `themer` useful, here are some ways to support the project:

* Star [`themer` on GitHub](https://github.com/mjswensen/themer)
* Follow [@themerdev](https://twitter.com/themerdev) on Twitter
* [Send a tip through the Brave Browser](https://brave.com/the537), either on [the repository page](https://github.com/mjswensen/themer) or [the Web UI](https://themer.dev)
* Pay what you want when downloading your theme from [themer.dev](https://themer.dev)

# Installation instructions

## Alacritty

1. Paste the contents of `Alacritty/Themer.yml` into your Alacritty config file.
2. Select the desired theme by setting the `colors` config key to reference the scheme's anchor (i.e., `colors: *light` or `colors: *dark`).

## Brave

1. Launch Brave and go to `brave://extensions`.
2. Check the "Developer mode" checkbox at the top.
3. Click the "Load unpacked extension..." button and choose the desired theme directory (`Brave/Themer Dark` or `Brave/Themer Light`).

(To reset or remove the theme, visit `brave://settings` and click "Reset to Default" in the "Appearance" section.)

## Burst Wallpaper

Files generated:

* `Burst Wallpaper/themer-wallpaper-burst-dark-1526x690.png`
* `Burst Wallpaper/themer-wallpaper-burst-light-1526x690.png`

## Chrome

1. Launch Chrome and go to `chrome://extensions`.
2. Check the "Developer mode" checkbox at the top.
3. Click the "Load unpacked extension..." button and choose the desired theme directory (`Chrome/Themer Dark` or `Chrome/Themer Light`).

(To reset or remove the theme, visit `chrome://settings` and click "Reset to Default" in the "Appearance" section.)

## CMD

Simply double-click the desired theme file to add the color keys to the registry:

* `CMD/themer-dark.reg`
* `CMD/themer-light.reg`

The scheme of CMD can then be configured with the `color` command. For example, use `color 07` to set the background and foreground to your color set's default.

## CSS

Import the generated theme file into your stylesheet via `@import()`, or into your HTML markup via `<link>`.

`hex.css` provides the theme colors in hex format; `rgb.css` and `hsl.css` in RGB and HSL formats respectively along with individual channel values for further manipulation if desired.

Generated files:

* `CSS/hex.css`
* `CSS/rgb.css`
* `CSS/hsl.css`

## Emacs

Copy (or symlink) the generated theme files into `~/.emacs.d/`:

    cp 'Emacs/themer-dark-theme.el' ~/.emacs.d/
    cp 'Emacs/themer-light-theme.el' ~/.emacs.d/

Then load the desired theme in `init.el`:

    (load-theme 'themer-dark t)
    ;; or
    (load-theme 'themer-light t)

## Firefox Add-on

To use the generated extension package, the code will need to be packaged up and signed by Mozilla.

To package the code in preparation for submission, the `web-ext` tool can be used:

    npx web-ext build --source-dir 'Firefox Add-on/Themer Dark' # or 'Firefox Add-on/Themer Light'

Then the package can be submitted to Mozilla for review in the [Add-on Developer Hub](https://addons.mozilla.org/en-US/developers/addon/submit/distribution).

Learn more about Firefox themes from [extensionworkshop.com](https://extensionworkshop.com/documentation/themes/)

To theme Firefox without the need to create a developer account and go through the extension review process, see themer's integration with [Firefox Color](https://color.firefox.com).

## Firefox Color

The Firefox Color add-on allows for simple theming without the need for a developer account or package review process by Mozilla.

1. Install the [Firefox Color add-on](https://addons.mozilla.org/en-US/firefox/addon/firefox-color/).
2. Open 'Firefox Color/themer-dark.url' or 'Firefox Color/themer-light.url' directly with Firefox.
3. Click "Yep" when prompted to apply the custom theme.

For a more fully featured Firefox theme, see themer's Firefox theme add-on generator.

## kitty

In the kitty configuration file (usually `~/.config/kitty/kitty.conf`), `include` the generated theme file:

    include kitty/themer-dark.conf
    include kitty/themer-light.conf

## Konsole

Copy (or symlink) the generated files to `~/.local/share/konsole/`:

    cp 'Konsole/themer-dark.colorscheme' ~/.local/share/konsole/
    cp 'Konsole/themer-light.colorscheme' ~/.local/share/konsole/

Then choose the desired theme in Konsole > Settings > Edit Current Profile > Appearance.

## Octagon Wallpaper

Files generated:

* `Octagon Wallpaper/themer-wallpaper-octagon-dark-1526x690.png`
* `Octagon Wallpaper/themer-wallpaper-octagon-light-1526x690.png`

## Sublime Text

1. Copy (or symlink) the generated theme files (`Sublime Text/themer-sublime-text-dark.tmTheme` or `Sublime Text/themer-sublime-text-light.tmTheme`) to the `User/` packages folder (you can see where this folder is located by choosing the "Browse Packages..." menu option in Sublime Text).
2. Choose the theme from the list of available color themes.

## Terminator

Copy the contents of `Terminator/themer-terminator-dark.txt` or `Terminator/themer-terminator-light.txt` to the Terminator's config file.

The config file is usually located at `~/.config/terminator/config`.

You can paste it as a new profile, or copy the contents into your existing profile.

Finally, restart Terminator to see the new theme.

## Trianglify Wallpaper

Files generated:

* `Trianglify Wallpaper/themer-wallpaper-trianglify-dark-1526x690-0.75-1.png`
* `Trianglify Wallpaper/themer-wallpaper-trianglify-dark-1526x690-0.75-2.png`
* `Trianglify Wallpaper/themer-wallpaper-trianglify-light-1526x690-0.75-1.png`
* `Trianglify Wallpaper/themer-wallpaper-trianglify-light-1526x690-0.75-2.png`

## Vim

Copy or symlink `Vim/ThemerVim.vim` to `~/.vim/colors/`.

Then set the colorscheme in `.vimrc`:

    " The background option must be set before running this command.
    colo ThemerVim

## Visual Studio

1. Select Tools > Import and Export Settings...
2. Choose the "Import selected environment settings" option
3. Choose whether or not to save a backup of current settings
4. Click "Browse..." and choose the generated theme file ('Visual Studio/themer-dark.vssettings' or 'Visual Studio/themer-light.vssettings')
5. Click "Finish"

## VS Code

Copy (or symlink) the generated package directory into the VS Code extensions directory:

    cp -R 'VS Code/theme-themer-vscode' ~/.vscode/extensions/

Then reload or restart VS Code. The generated theme package should be in the list of installed extensions, and "Themer Dark" / "Themer Light" will be available in the list of themes.