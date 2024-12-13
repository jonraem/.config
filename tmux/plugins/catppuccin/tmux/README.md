<!-- markdownlint-disable -->
<h3 align="center">
 <img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/logos/exports/1544x1544_circle.png" width="100" alt="Logo"/><br/>
 <img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/misc/transparent.png" height="30" width="0px"/>
 Catppuccin for <a href="https://github.com/tmux/tmux">Tmux</a>
 <img src="https://raw.githubusercontent.com/catppuccin/catppuccin/main/assets/misc/transparent.png" height="30" width="0px"/>
</h3>

<p align="center">
    <a href="https://github.com/catppuccin/tmux/stargazers"><img src="https://img.shields.io/github/stars/catppuccin/tmux?colorA=363a4f&colorB=b7bdf8&style=for-the-badge"></a>
    <a href="https://github.com/catppuccin/tmux/issues"><img src="https://img.shields.io/github/issues/catppuccin/tmux?colorA=363a4f&colorB=f5a97f&style=for-the-badge"></a>
    <a href="https://github.com/catppuccin/tmux/contributors"><img src="https://img.shields.io/github/contributors/catppuccin/tmux?colorA=363a4f&colorB=a6da95&style=for-the-badge"></a>
</p>

<!-- markdownlint-enable -->

> [!NOTE]
> These files have been modified by the forker. Please visit the [Catppucin for Tmux](https://github.com/catppuccin/tmux) repository for updates.

## Installation

In order to have the icons displayed correctly please use/update your favorite
[Nerd Font](https://www.nerdfonts.com/font-downloads).
If you do not have a patched font installed, you can override or remove any
icon. Check the [documentation](./docs/reference/configuration.md) on the
options available.

### Manual (Recommended)

This method is recommended as TPM has some issues with name conflicts.

<!-- x-release-please-start-version -->
1. Clone this repository to your desired location (e.g.
   `~/.config/tmux/plugins/catppuccin`).

    ```bash
    mkdir -p ~/.config/tmux/plugins/catppuccin
    git clone -b v2.1.2 https://github.com/catppuccin/tmux.git ~/.config/tmux/plugins/catppuccin/tmux
    ```

1. Add the following line to your `tmux.conf` file:
   `run ~/.config/tmux/plugins/catppuccin/tmux/catppuccin.tmux`.
1. Reload Tmux by either restarting or reloading with `tmux source ~/.tmux.conf`.
<!-- x-release-please-end -->

Check out what to do next in the "[Getting Started Guide](./docs/tutorials/01-getting-started.md)".

### TPM

<!-- x-release-please-start-version -->
1. Install [TPM](https://github.com/tmux-plugins/tpm)
1. Add the Catppuccin plugin:

    ```bash
    set -g @plugin 'catppuccin/tmux#v2.1.2' # See https://github.com/catppuccin/tmux/tags for additional tags
    # ...alongside
    set -g @plugin 'tmux-plugins/tpm'
    ```

1. (Optional) Set your preferred flavor, it defaults to `"mocha"`:

    ```bash
    set -g @catppuccin_flavor 'mocha' # latte, frappe, macchiato or mocha
    ```
<!-- x-release-please-end -->

> [!IMPORTANT]
> You may have to run `~/.config/tmux/plugins/tpm/bin/clean_plugins`
> if upgrading from an earlier version
> (especially from `v0.3.0`).

## Documentation

### Guides

- [Getting Started](./docs/tutorials/01-getting-started.md)
- [Custom Status Line Segments](./docs/tutorials/02-custom-status.md)

### Reference

- [Status Line](./docs/reference/status-line.md)
- [Configuration Options Reference](./docs/reference/configuration.md)
- [Tmux Configuration Showcase](https://github.com/catppuccin/tmux/discussions/317)

