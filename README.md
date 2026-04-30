# Dotfiles

## Installation & Uninstallation

```shell
./bin/install.sh
```

```shell
./bin/uninstall.sh
```

## Instructions

### Creating source files

Any file which matches the shell glob `_*` will be linked into `$HOME` as a symlink with the first `_`  replaced with a `.`

For example:

```bash
_bashrc
```

becomes

```bash
${HOME}/.bashrc
```

I've extended the `install.sh` script to handle `.config` directory, too. Just create a directory named `_config` and add files or directories in this directory. Everything inside `_config` will be symlinked to `.config`.
