
## Setup and Config

git - Content tracker
```
git [--version] [--help] [-C <path>] [-c <name>=<value>]
    [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
    [-p|--paginate|-P|--no-pager] [--no-replace-objects] [--bare]
    [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
    [--super-prefix=<path>] [--config-env=<name>=<envvar>]
    <command> [<args>]
```
config - Get and set repository or global options
```
git config [<file-option>] [--type=<type>] [--fixed-value] [--show-origin] [--show-scope] [-z|--null] name [value [value-pattern]]
```
help - Display help information about Git
```
git help [-a|--all [--[no-]verbose]] [-g|--guides]
	   [-i|--info|-m|--man|-w|--web] [COMMAND|GUIDE]
```
bugreport - Collect information for user to file a bug report
```
git bugreport [(-o | --output-directory) <path>] [(-s | --suffix) <format>]
```

## Getting and Creating Projects

init - Create an empty Git repository or reinitialize an existing one

```
git init [-q | --quiet] [--bare] [--template=<template_directory>]
	  [--separate-git-dir <git dir>] [--object-format=<format>]
	  [-b <branch-name> | --initial-branch=<branch-name>]
	  [--shared[=<permissions>]] [directory]
```
clone - Clone a repository into a new directory

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

## Basic Snapshotting

add - Add file contents to the index
```
git add [--verbose | -v] [--dry-run | -n] [--force | -f] [--interactive | -i] [--patch | -p]
	  [--edit | -e] [--[no-]all | --[no-]ignore-removal | [--update | -u]]
	  [--intent-to-add | -N] [--refresh] [--ignore-errors] [--ignore-missing] [--renormalize]
	  [--chmod=(+|-)x] [--pathspec-from-file=<file> [--pathspec-file-nul]]
	  [--] [<pathspec>…​]
```
status - Show the working tree status
```
git status [<options>…​] [--] [<pathspec>…​]
```
diff - Show changes between commits, commit and working tree, etc
```
git diff [<options>] [<commit>] [--] [<path>…​]
```
commit - Record changes to the repository
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
notes - Add or inspect object notes
```
git notes [list [<object>]]
```
restore - Restore working tree files
```
git restore [<options>] [--source=<tree>] [--staged] [--worktree] [--] <pathspec>…
```
reset - Reset current HEAD to the specified state
```
git reset [-q] [<tree-ish>] [--] <pathspec>…​
```
rm - Remove files from the working tree and from the index
```
git rm [-f | --force] [-n] [-r] [--cached] [--ignore-unmatch]
	  [--quiet] [--pathspec-from-file=<file> [--pathspec-file-nul]]
	  [--] [<pathspec>…​]
```
mv - Move or rename a file, a directory, or a symlink
```
git mv <options>…​ <args>…​
```

## Branching and Merging

branch
checkout
switch
merge
mergetool
log
stash
tag
worktree

## Sharing and Updating Projects

fetch
pull
push
remote
submodule

## Inspection and Comparison

show
log
diff
difftool
range-diff
shortlog
describe

## Patching
apply
cherry-pick
diff
rebase
revert

## Debugging
bisect
blame
grep

## Guides
gitattributes
Command-line interface conventions
Everyday Git
Frequently Asked Questions (FAQ)
Glossary
Hooks
gitignore
gitmodules
Revisions
Submodules
Tutorial
Workflows
All guides...

## Email
am
apply
format-patch
send-email
request-pull

## External Systems
svn
fast-import

## Administration
clean
gc
fsck
reflog
filter-branch
instaweb
archive
bundle

## Server Admin
daemon
update-server-info

## Plumbing Commands
cat-file
check-ignore
checkout-index
commit-tree
count-objects
diff-index
for-each-ref
hash-object
ls-files
ls-tree
merge-base
read-tree
rev-list
rev-parse
show-ref
symbolic-ref
update-index
update-ref
verify-pack
write-tree
