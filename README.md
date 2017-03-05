# Introduction
elementaryOS Post Install Tool (ePIT for short) is a fork of [Fedy](http://folkswithhats.org/). It lets you install multimedia codecs and additional software that elementary OS doesn't ship, like Steam, Spotify, Google Chrome, and much more with just a few clicks.

## License
This program is free software: you can redistribute it and/or modify it under the terms of the GNU General Public License as published by the Free Software Foundation, either version 3 of the License, or (at your option) any later version.

This program is distributed in the hope that it will be useful, but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.

You should have received a copy of the GNU General Public License along with this program.  If not, see [gnu.org/licenses](http://www.gnu.org/licenses/).

Copyright (C) [Satyajit Sahoo](mailto:satyajit.happy@gmail.com)

## Usage
ePIT can be installed with the following command :
```bash
curl https://raw.githubusercontent.com/monsieurh/elementaryPIT/master/installer.sh | sudo bash
```

# User
After installation, search for `ePIT` in the menu.

# Contributor
There are several ways to contribute. You can :

- [report bugs](https://github.com/monsieurh/elementaryPIT/issues)
- [suggest features](https://github.com/monsieurh/elementaryPIT/issues)
- code
- help translating/documenting

## Developer

### Plugin structure
Plugins can be placed under `~/.local/share/epit/plugins/`, or the system plugins directory.

Each plugin is a directory with the suffix `.plugin`, which consist of a JSON formatted metadata file. The metadata file contains information about the plugin and describes how `Fedy` should run the tasks.

The plugins can run any command or scripts (`bash`, `python` etc.). In addition to the system commands, `Fedy` provides an additional command, `run-as-root` to allow running commands (e.g.- `run-as-root touch /some/file/somewhere`) or scripts (e.g.- `run-as-root -s do-stuff.sh`) as root.

Have a look at the existing plugins to know more about how to write plugins for `Fedy`.

### Source cod
You can get the latest source code from the [github page](https://github.com/monsieurh/elementaryPIT).

`git clone https://github.com/monsieurh/elementaryPIT`

### Bugs and feature requests
Please submit bugs and feature requests [here](https://github.com/monsieurh/elementaryPIT/issues). Pull requests are always welcome.
