zsh-rustup-completion
---------------------

Oh-my-zsh rustup completion plugin.

Rustup version: **1.44.0** (b8cedc004 2020-03-09)

## Installation

First clone the repository repo in the custom zsh plugins folder:

### Zinit
Open ~/.zshrc
```bash
vim ~/.zshrc
```

Add the plugin to zinit
```bash
zinit lucid wait for \
  atinit"zicompinit; zicdreplay" \
    Arzte/zsh-rustup-completion
```

### Oh-My-Zsh

```bash
cd ~/.oh-my-zsh/custom/plugins
git clone https://github.com/Arzte/zsh-rustup-completion.git rustup
```

Open ~/.zshrc:

```bash
vim ~/.zshrc
```

Add the plugin to zsh:
```bash
plugins=(... rustup)
```

Check that autoloading is enabled:
```bash
autoload -U compinit && compinit
```

Reload config:
```bash
source ~/.zshrc
```

Enjoy it!

## Updating

Completion file depends on rustup version.
For updating completion just execute:

```bash
./gen-completion.sh
```

Attention! Executing this file may cause repo updating failure.
