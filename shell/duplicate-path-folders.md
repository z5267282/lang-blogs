# Overview

The folders in `$PATH` are getting duplicated.  
I am trying to find out why.

Theories:

| no. | desc                                      |
| --- | ----------------------------------------- |
| 1   | `.zshrc` is getting run twice             |
| 2   | some other `zsh` file is running it twice |

# Hunch

The issue is that folders like

```sh
/Users/sunny/OneDrive - UNSW/UNSW/Courses/Year 5 - 2023/seng3011
```

are getting recorded twice.  
These are only ever set in `~/.zshrc` so I know it is getting run twice.

# Solution

The following command can remove duplicate items from `$PATH`

```sh
typeset -U path
```

Link [here](https://tech.serhatteker.com/post/2019-12/remove-duplicates-in-path-zsh/)
