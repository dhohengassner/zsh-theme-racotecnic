Racó Tècnic ZSH Theme
=====================

ZSH theme based on Andy Fleming's theme [af-magic](https://coderwall.com/p/3xcpyg) and inspired by the [posh-git](https://github.com/dahlbyk/posh-git) features.

![screenshot](screenshot.png)

Installing
----------

As oh-my-zsh is not accepting more themes right now, you will need to manually download and install the theme in your themes folder.

The Prompt
----------

The prompt is similar to the posh-git prompt with two little differences:

- The zeros have been removed, in order to give up some space to the term.
- If you have stashed changes it will appear an asterisk in the right side of the left prompt.

The status summary has the following format:

    [{HEAD-name} +A ~B -C !D | +E ~F -G !H *]

* `{HEAD-name}` is the current branch, or the SHA of a detached HEAD
 * Blue means the branch matches its remote
 * Green means the branch is ahead of its remote (green light to push)
 * Red means the branch is behind its remote
 * Yellow means the branch is both ahead of and behind its remote
* ABCD represent the index; EFGH represent the working directory
 * `+` = Added files
 * `~` = Modified files
 * `-` = Removed files
 * `!` = Conflicted files
 * As in `git status`, index status is dark green and working directory status is dark red
* An asterisk `*` represents stashed changes

Based on work by
----------------

- [Keith Dahlby (posh-git)](https://github.com/dahlbyk)
- [Andy Fleming (af-magic theme)](https://github.com/andyfleming)
