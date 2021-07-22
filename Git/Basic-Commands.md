
## git-clone ##
Clone a repository into a new directory
```
git clone [--template=<template_directory>]
	  [-l] [-s] [--no-hardlinks] [-q] [-n] [--bare] [--mirror]
	  [-o <name>] [-b <name>] [-u <upload-pack>] [--reference <repository>]
	  [--dissociate] [--separate-git-dir <git dir>]
	  [--depth <depth>] [--[no-]single-branch] [--no-tags]
	  [--recurse-submodules[=<pathspec>]] [--[no-]shallow-submodules]
	  [--[no-]remote-submodules] [--jobs <n>] [--sparse] [--[no-]reject-shallow]
	  [--filter=<filter>] [--] <repository>
	  [<directory>]
```
  
 Eg: Clone from upstream:
$ git clone git://git.kernel.org/pub/scm/.../linux.git my-linux
$ git clone ssh://[user@]host.xz[:port]/~[user]/path/to/repo.git/

## git-fetch ##
Download objects and refs from another repository
```
git fetch [<options>] [<repository> [<refspec>…​]]
git fetch [<options>] <group>
git fetch --multiple [<options>] [(<repository> | <group>)…​]
git fetch --all [<options>]
```

Eg:
$ git fetch origin


## git-pull ##
Fetch from and integrate with another repository or a local branch
```
git pull [<options>] [<repository> [<refspec>…​]]
```

Eg:
$ git pull
$ git pull origin

## git-status ##
Show the working tree status

```
git status [<options>…​] [--] [<pathspec>…​]
```

## git-ignore##
Specifies intentionally untracked files to ignore
```
$XDG_CONFIG_HOME/git/ignore, $GIT_DIR/info/exclude, .gitignore
```
 Eg:
 $ cat .gitignore
    # exclude everything except directory foo/bar
    /*
    !/foo
    /foo/*
    !/foo/bar

## git-add ##
Add file contents to the index
```
git add [--verbose | -v] [--dry-run | -n] [--force | -f] [--interactive | -i] [--patch | -p]
	  [--edit | -e] [--[no-]all | --[no-]ignore-removal | [--update | -u]]
	  [--intent-to-add | -N] [--refresh] [--ignore-errors] [--ignore-missing] [--renormalize]
	  [--chmod=(+|-)x] [--pathspec-from-file=<file> [--pathspec-file-nul]]
	  [--] [<pathspec>…​]
```

Eg:Adds content from all *.txt files under Documentation directory and its subdirectories:

$ git add Documentation/\*.txt

## git-commit ##
Record changes to the repository
```
git commit [-a | --interactive | --patch] [-s] [-v] [-u<mode>] [--amend]
	   [--dry-run] [(-c | -C | --squash) <commit> | --fixup [(amend|reword):]<commit>)]
	   [-F <file> | -m <msg>] [--reset-author] [--allow-empty]
	   [--allow-empty-message] [--no-verify] [-e] [--author=<author>]
	   [--date=<date>] [--cleanup=<mode>] [--[no-]status]
	   [-i | -o] [--pathspec-from-file=<file> [--pathspec-file-nul]]
	   [(--trailer <token>[(=|:)<value>])…​] [-S[<keyid>]]
	   [--] [<pathspec>…​]
 ```
 

## git-merge ##
Join two or more development histories together

```
git merge [-n] [--stat] [--no-commit] [--squash] [--[no-]edit]
	[--no-verify] [-s <strategy>] [-X <strategy-option>] [-S[<keyid>]]
	[--[no-]allow-unrelated-histories]
	[--[no-]rerere-autoupdate] [-m <msg>] [-F <file>] [<commit>…​]
git merge (--continue | --abort | --quit)

```
Eg:
Merge branches fixes and enhancements on top of the current branch, making an octopus merge:

$ git merge fixes enhancements






