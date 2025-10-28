# fish-brew

Fork of [TacoMilkshake/fish-plugin-brew](https://github.com/TacoMilkshake/fish-plugin-brew) with LinuxBrew support, combined with [ohmyzsh/brew](https://github.com/ohmyzsh/ohmyzsh/tree/master/plugins/brew) ported to the Fish shell.

### Installation

Install with [fisher](https://github.com/jorgebucaran/fisher):

```shell
fisher install givensuman/fish-brew
```

### Usage

Initializes `brew` with necessary functions and completions for Fish.

Set the `brew_location` environment variable to specify an alternate `brew` location.

```shell
set --global brew_location /home/linuxbrew/.linuxbrew/bin/brew
```

### Aliases

There's a lot...
Note commands containing `--cask` will only work on MacOS.

| Alias  | Command                               | Description                                                           |
| ------ | ------------------------------------- | --------------------------------------------------------------------- |
| bl     | bleaves                               | Run custom `bleaves` function.                                        |
| bi     | brew install                          | Install a formula.                                                    |
| ba     | brew autoremove                       | Uninstall unnecessary formulae.                                       |
| bcfg   | brew config                           | Show Homebrew and system configuration info useful for debugging.     |
| bci    | brew info --cask                      | Display information about the given cask.                             |
| bcin   | brew install --cask                   | Install the given cask.                                               |
| bcl    | brew list --cask                      | List installed casks.                                                 |
| bcn    | brew cleanup                          | Run cleanup.                                                          |
| bco    | brew outdated --cask                  | Report all outdated casks.                                            |
| bcrin  | brew reinstall --cask                 | Reinstall the given cask.                                             |
| bcubc  | brew upgrade --cask && brew cleanup   | Upgrade outdated casks, then run cleanup.                             |
| bcubo  | brew update && brew outdated --cask   | Update Homebrew data, then list outdated casks.                       |
| bcup   | brew upgrade --cask                   | Upgrade all outdated casks.                                           |
| bdr    | brew doctor                           | Check your system for potential problems.                             |
| bfu    | brew upgrade --formula                | Upgrade only formulae (not casks).                                    |
| bi     | brew install                          | Install a formula.                                                    |
| bl     | brew list                             | List all installed formulae.                                          |
| bo     | brew outdated                         | List installed formulae that have an updated version available.       |
| brewp  | brew pin                              | Pin a specified formula so that it's not upgraded.                    |
| brews  | brew list -1                          | List installed formulae or the installed files for a given formula.   |
| brewsp | brew list --pinned                    | List pinned formulae, or show the version of a given formula.         |
| bs     | brew search                           | Perform a substring search of cask tokens and formula names for text. |
| bsl    | brew services list                    | List all running services.                                            |
| bsoff  | brew services stop                    | Stop the service and unregister it from launching at login (or boot). |
| bsoffa | bsoff --all                           | Stop all started services.                                            |
| bson   | brew services start                   | Start the service and register it to launch at login (or boot).       |
| bsona  | bson --all                            | Start all stopped services.                                           |
| bsr    | brew services run                     | Run the service without registering to launch at login (or boot).     |
| bsra   | bsr --all                             | Run all stopped services.                                             |
| bu     | brew update                           | Update brew and all installed formulae.                               |
| bubo   | brew update && brew outdated          | Update Homebrew data, then list outdated formulae and casks.          |
| bubu   | bubo && bup                           | Do the last two operations above.                                     |
| bugbc  | brew upgrade --greedy && brew cleanup | Upgrade outdated formulae and casks (greedy), then run                | cleanup | .   |
| bup    | brew upgrade                          | Upgrade outdated, unpinned brews.                                     |
| buz    | brew uninstall --zap                  | Remove all files associated with a cask.                              |

### Requirements

Just requires [brew](https://brew.sh/)!

### License

[MIT](../LICENSE)

