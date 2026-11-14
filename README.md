# Dotfiles

My personal Linux desktop configuration, built around the [niri](https://github.com/YaLTeR/niri) scrollable-tiling Wayland compositor and [Noctalia Shell](https://github.com/noctalia-dev/noctalia-shell) for the bar, launcher and notifications.


## What's inside

| Component | Tool |
|---|---|
| Compositor | niri |
| Shell (bar, launcher, notifications) | Noctalia Shell |
| Terminal | [kitty] |
| Shell | [zsh] |
| Editor | [vim VS Codium] |
| Fonts | [JetBrains-Mono-Nerd-fonts] |
| Distro | [Fedora]|

## Repository structure

```
Dotfiles/
├── Niri/            # niri config (KDL): keybindings, layout, window rules      # Noctalia Shell settings and theme
├── Kitty/      # terminal config
├── fastfetch #fastfetch configuration
├── rofi # rofi themeing and configuration
```

## Highlights

- **Custom keybindings** for a fully keyboard-driven workflow (see the table below)
- **Unified theme** across the bar, launcher and notifications via Noctalia

## Key bindings

| Shortcut | Action |
|---|---|
| `Mod + T` | Open terminal |
| `Mod + Q` | Close window |
| `Ctrl + Space` | Show Noctalia Application launcher  |


## Installation

> Back up your existing config before copying anything.

1. Install the dependencies: `niri`, `noctalia-shell`, [other packages].

2. Clone the repo:

   ```bash
   git clone https://github.com/Night-Crypt/Dotfiles.git ~/Dotfiles
   cd ~/Dotfiles
   ```

3. Link the configs into place (using GNU Stow, or `ln -s` manually):

   ```bash
   stow niri noctalia
   ```

4. Log out and select **niri** from your display manager, or start it from a TTY with `niri-session`.

## Notes

- Tested on [Fedora 44].
- Some paths and keybindings are specific to my hardware (e.g. [monitor, keyboard layout]). Adjust them for your setup.

## Credits

- [niri](https://github.com/YaLTeR/niri) by YaLTeR
- [Noctalia Shell](https://github.com/noctalia-dev/noctalia-shell)
- [Any configs or wallpapers you borrowed from]

## License

[MIT, or "Personal configs, use freely" if you don't care.]
