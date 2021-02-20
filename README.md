# dictd-dictionaries

This repository contains a large number of dictionary files from Ubuntu
repository, which can be used for `dictd` server.

This helps people whose distro doesn't deliver the packages for dictd dictionaries.

If you find another missing dictionary feel free to file an issue or a pull request.

## How to install

- Find the databases and indexes of dictionaries you want to install in the release
- Copy `*.dict.dz` and `*.index` files to `/usr/share/dictd`
- Include `db.list` in your dictd config file, such as `/etc/dictd.config`
