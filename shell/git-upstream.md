# Overview

How to fix this problem:

```
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.
```

. Run this:

```sh
git config --global --add --bool push.autoSetupRemote true
```

from [here](https://stackoverflow.com/questions/29422101/automatically-track-remote-branch-with-git).