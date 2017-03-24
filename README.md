# Kraemls dotfiles

`using Git, GNU stow and Ansible`

Do not use this directly, but take parts and learn from it. I share it because I got frustrated about moving a tarball around (and being scared of loosing it). Which eventually happened when my notebook got stolen... so, this is not an ideal solution yet. It only contains the basic from an old tarball, and still needs all the customization for vim, emacs, etc. For now, No support, no comments, nothing... "what you see is what it is"...

## Requirements

CentOS/Fedora

```
$ yum install git tmux zsh mc stow #dnf
```

Debian/Ubuntu

```
$ apt-get install git tmux zsh mc stow
```

After this you can use GNU `stow` to install the dotfiles per application

```
$ git clone https://github.com/kraeml/dotfiles.git .dotfiles --recursive
$ cd .dotfiles
$ stow zsh
```

## Installation

### Shell script

```
$ curl -sSL https://raw.githubusercontent.com/kraeml/dotfiles/master/install.sh | sh
```

### Ansible

This has been tested with Ansible 2.0+.

```
$ curl -sSL https://raw.githubusercontent.com/kraeml/dotfiles/master/install.yml -o install.yml
```

```
$ chmod u+x install.yml
$ ./install.yml
```

or

```
$ ansible-playbook install.yml
```

## Authors

| [!["Gerard Braad"](http://gravatar.com/avatar/e466994eea3c2a1672564e45aca844d0.png?s=60)](http://gbraad.nl "Gerard Braad <me@kraeml.nl>")
| -----------------------------------------------------------------------------------------------------------------------------------------
| [@gbraad](https://twitter.com/kraeml)
