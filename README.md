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

### Requirements

Just requires [brew](https://brew.sh/)!

### License

[MIT](../LICENSE)
