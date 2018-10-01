
# About

**prepare-commit-message** adds to commit message branch name, which can be parsed be Bitbucket. It works with every git's GUIs. 
If you work on Windows you should install [grep](http://gnuwin32.sourceforge.net/packages/grep.htm), [awk](http://gnuwin32.sourceforge.net/packages/gawk.htm) and [sed](http://gnuwin32.sourceforge.net/packages/sed.htm) tool.

# Getting started

## Installation

To install globally, copy `prepare-commit-msg` to `/usr/local/share/git-core/templates/hooks` and execute:

```
chmod +x /usr/local/share/git-core/templates/hooks/prepare-commit-msg
```

To install per-repository, copy `prepare-commit-msg` to `/path/to/repo/.git/hooks/prepare-commit-msg` and mark it as executable.

Hooks need to be executable, so you may need to change the file permissions of the script if you’re creating it from scratch. For example, to make sure that prepare-commit-msg is executable, you would run the following command:

```
chmod +x prepare-commit-msg
```

## Usage

The branch name will be automatically appended to commit messages using `git commit` or `git commit -m "message"`.

## Notes

If you'd like to use this commit message hook in an existing repository, after copying the file to the proper location, run `git init` within the repository for the hook to be initialized.

# Thanks

On the basis of [Jim Schubert's](https://gist.github.com/jimschubert/9073276) code.
