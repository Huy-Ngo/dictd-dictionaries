# dictd-dictionaries

This repository contains a large number of dictionary files from Ubuntu
repository, which can be used for `dictd` server.

This helps people whose distro doesn't deliver the packages for dictd dictionaries.

If you find another missing dictionary feel free to file an issue or a pull request.

## How to install

- Find the databases and indexes of dictionaries you want to install in the release
- Copy `*.dict.dz` and `*.index` files to `/usr/share/dictd`
- Include `db.list` in your dictd config file, such as `/etc/dictd.config`

## Available dictionaries

- Various dictionaries distributed for Ubuntu repo: gcide, WordNet, Moby Thesaurus,
  FreeDictionaries, VERA, Jargon
- Wiktionary, based on [NixOS package][nixos]

[nixos]: https://github.com/NixOS/nixpkgs/tree/master/pkgs/servers/dict/wiktionary

## Why use Git commits and messy branches?

Yes I know git is not for storing files, but apparently using release has limited API call,
and I can't push to the same branch because of concurency problem.
