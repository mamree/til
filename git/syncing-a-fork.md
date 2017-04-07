# Syncing a Fork

List the current configured remote repository for your fork.

```bash
git remote -v
```

Specify new remote `upstream` that will be synced with the fork:

```bash
git remote add upstream https://github.com/rails/rails.git
```

Verity the new upstream added:

```bash
$ git remote -v
origin ... (fetch)
origin ... (push)
upstream ... (fetch)
upstream ... (push)
```

Keep it updated:

```bash
$ git fetch upstream
$ git checkout master
$ git merge upstream/master
```

## References:

* https://help.github.com/articles/configuring-a-remote-for-a-fork/
* https://help.github.com/articles/syncing-a-fork/
