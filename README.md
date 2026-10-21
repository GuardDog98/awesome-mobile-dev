# awesome-mobile-dev
A curated list of tools and workflows for coding and building software from your phone (Termux and Android).


# Awesome Mobile Dev [

![Awesome](https://awesome.re/badge.svg)

](https://awesome.re)

> A curated list of tools, guides and workflows for **writing, building and shipping software from your phone**, with a focus on [Termux](https://github.com/termux/termux-app) on Android.

No laptop? No problem. This list collects what actually works on a phone.

Contributions are welcome. Please read the [contribution guidelines](#contributing) first.

## Contents

- [Getting Started](#getting-started)
- [Terminal Emulators and Core Apps](#terminal-emulators-and-core-apps)
- [Editors and IDEs](#editors-and-ides)
- [Shells and Productivity](#shells-and-productivity)
- [Version Control and CI](#version-control-and-ci)
- [Languages and Runtimes](#languages-and-runtimes)
- [Android Development on Android](#android-development-on-android)
- [Linux Distros and Desktop](#linux-distros-and-desktop)
- [Remote Access](#remote-access)
- [Tips and Workflows](#tips-and-workflows)
- [Contributing](#contributing)

## Getting Started

- [Termux Wiki](https://wiki.termux.com) - Official documentation: package management, storage access, API usage.
- [Termux on GitHub](https://github.com/termux/termux-app) - The terminal emulator and Linux environment for Android.
- [Termux Packages](https://github.com/termux/termux-packages) - Build scripts for every package available through `pkg`.
- [F-Droid](https://f-droid.org) - Recommended source for installing Termux and its plugins (keep all Termux apps from the same source).

## Terminal Emulators and Core Apps

- [Termux:API](https://github.com/termux/termux-api) - Access Android features (clipboard, notifications, sensors, SMS) from the shell.
- [Termux:Boot](https://github.com/termux/termux-boot) - Run scripts when the device boots.
- [Termux:Widget](https://github.com/termux/termux-widget) - Start shell scripts from the home screen.
- [Termux:Styling](https://github.com/termux/termux-styling) - Color schemes and fonts for Termux.
- [Termux:Tasker](https://github.com/termux/termux-tasker) - Run Termux commands from Tasker.

## Editors and IDEs

- [Neovim](https://neovim.io) - Modal editor, available via `pkg install neovim`.
- [Helix](https://helix-editor.com) - Modern modal editor with built-in LSP support.
- [Micro](https://micro-editor.github.io) - Beginner-friendly terminal editor with familiar shortcuts.
- [code-server](https://github.com/coder/code-server) - VS Code in the browser, usable on a phone via a local server.
- [Acode](https://github.com/Acode-Foundation/Acode) - Code editor app for Android with plugin support.

## Shells and Productivity

- [Zsh](https://www.zsh.org) and [Oh My Zsh](https://github.com/ohmyzsh/ohmyzsh) - Popular shell and configuration framework.
- [Fish](https://fishshell.com) - Friendly interactive shell with good defaults.
- [Starship](https://starship.rs) - Fast, customizable prompt.
- [tmux](https://github.com/tmux/tmux) - Terminal multiplexer, very useful on small screens with extra keys.
- [fzf](https://github.com/junegunn/fzf) - Fuzzy finder for files and history.
- [ripgrep](https://github.com/BurntSushi/ripgrep) - Fast recursive search.
- [bat](https://github.com/sharkdp/bat) - `cat` with syntax highlighting.
- [htop](https://htop.dev) - Interactive process viewer.

## Version Control and CI

- [Git](https://git-scm.com) - `pkg install git`.
- [GitHub CLI](https://cli.github.com) - Manage repositories, pull requests and Actions from the terminal.
- [lazygit](https://github.com/jesseduffield/lazygit) - Terminal UI for Git.
- [GitHub Actions](https://docs.github.com/actions) - Build APKs in the cloud when your phone cannot (see [Tips](#tips-and-workflows)).

## Languages and Runtimes

- Python, Node.js, Go, Rust, Clang, Ruby and OpenJDK are available through `pkg`. Run `pkg search <name>` to see current versions.

## Android Development on Android

- [AndroidIDE](https://github.com/AndroidIDEOfficial/AndroidIDE) - IDE that builds Android projects on-device.
- [termux-ndk](https://github.com/lzhiyong/termux-ndk) - Prebuilt NDK for Termux (ARM).
- [android-sdk-tools](https://github.com/lzhiyong/android-sdk-tools) - Android SDK tools built for Termux (ARM).

## Linux Distros and Desktop

- [proot-distro](https://github.com/termux/proot-distro) - Install Debian, Ubuntu, Arch and more inside Termux without root.
- [Termux:X11](https://github.com/termux/termux-x11) - X server for running graphical Linux apps.

## Remote Access

- [OpenSSH](https://www.openssh.com) - `pkg install openssh` to SSH into your phone or out to a server.
- [Mosh](https://mosh.org) - Resilient shell sessions on unstable mobile connections.

## Tips and Workflows

- **Build without a PC:** Push your Android project to GitHub and let GitHub Actions build the APK, then download it from the run's Artifacts.
- **Access phone storage:** Run `termux-setup-storage` to link shared storage.
- **Keep sessions alive:** Use `tmux` and disable battery optimization for Termux.
- **Extra keys:** Customize the extra keys row in `~/.termux/termux.properties` for Esc, Tab, Ctrl and arrows.
- **Backups:** `tar` your `$HOME` regularly to shared storage.

## Contributing

Your contributions are always welcome!

- Add one item per pull request when possible.
- Every entry must be **actively maintained** and **confirmed to work on a phone**.
- Use the format: `- [Name](link) - Short description ending with a period.`
- Keep descriptions neutral, factual and short.
- Keep each section in alphabetical order, or by relevance if stated.
- No affiliate links, ads or self-promotion without real value.
- Check that your link is not already in the list.

## License

[

![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)

](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the contributors have waived all copyright and related rights to this work.