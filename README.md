# edu-rofi-themes

A bundle of [rofi](https://github.com/davatorium/rofi) themes (`*.rasi`) installed system-wide, ready to be selected from any rofi config. Pair with [edu-rofi](https://github.com/erikdubois/edu-rofi) for the matching launcher configuration. Part of the `~/EDU/` learning series.

## What's in this repo

- `usr/share/rofi/themes/` — rofi `.rasi` theme files that land in `/usr/share/rofi/themes/`.
- `setup.sh`, `up.sh` — standard EDU bash scaffold.

## Companion repo

- [edu-rofi](https://github.com/erikdubois/edu-rofi) — the matching launcher config (keybindings, helper scripts).

## Installation

### From `nemesis_repo` (recommended)

```ini
[nemesis_repo]
SigLevel = Never
Server = https://erikdubois.github.io/$repo/$arch
```

```bash
sudo pacman -Syu
sudo pacman -S edu-rofi-themes
```

### Manual

```bash
git clone https://github.com/erikdubois/edu-rofi-themes.git
cd edu-rofi-themes
sudo cp -r usr/share/rofi/themes/. /usr/share/rofi/themes/
```

### Using a theme

In your rofi config (`~/.config/rofi/config.rasi`):

```rasi
@theme "<theme-name-without-extension>"
```

Or via the CLI:

```bash
rofi -theme <theme-name> -show drun
```

## Websites

Information : https://erikdubois.be

## Social Media

Youtube : https://www.youtube.com/erikdubois

## License

See [LICENSE](./LICENSE).
