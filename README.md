# Nerd fontpatcher

```bash
$ docker run --rm -it iwai/nerd-fontpatcher
Copyright (c) 2000-2018 by George Williams. See AUTHORS for Contributors.
 License GPLv3+: GNU GPL version 3 or later <http://gnu.org/licenses/gpl.html>
 with many parts BSD <http://fontforge.org/license.html>. Please read LICENSE.
 Based on sources from 03:03 UTC 26-May-2019-ML-D.
 Based on source from git with hash: 1acfefab9484f70256f0ff47cd60ded3c3c69a06
usage: font-patcher [-h] [-v] [-s] [-l] [-q] [-w] [-c] [--fontawesome]
                    [--fontawesomeextension] [--fontlinux] [--octicons]
                    [--powersymbols] [--pomicons] [--powerline]
                    [--powerlineextra] [--material] [--weather]
                    [--custom [CUSTOM]] [--postprocess [POSTPROCESS]]
                    [--removeligs] [--configfile [CONFIGFILE]]
                    [--progressbars | --no-progressbars] [--careful]
                    [-ext [EXTENSION]] [-out [OUTPUTDIR]]
                    font
font-patcher: error: too few arguments
```

## Example

```bash
curl -sSfL -O https://www.rs.tus.ac.jp/yyusa/ricty_diminished/ricty_diminished-4.1.1.tar.gz

tar zxf ricty_diminished-4.1.1.tar.gz

docker run --rm -it -v $(pwd):/data iwai/nerd-fontpatcher --complete -out . /data/RictyDiminished-Regular.ttf
```
