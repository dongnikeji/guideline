![Git][git-logo]

## Overview

* [Basic](#basic)
* [Recommend Workflow](#recommend-workflow)
* [Common Commands](#common-commands)
* [How-to](#how-to)
* [Reference](#reference)

## Basic
1. You can download it in the following website: https://git-scm.com or you can install it through `brew` if you are using mac computers;

2. Useful gui clients for git repo management:
    - Mac OSX: [GitX](http://gitx.frim.nl/) (free), [Tower](http://www.git-tower.com/) (commerical);

    - Window: [GitHub for Windows](https://windows.github.com/), [SmartGit](http://www.syntevo.com/smartgit/)

3. [Git](https://github.com/kemayo/sublime-text-git) and [Git Gutter](https://github.com/jisaacks/GitGutter) packages are good to have if you are using [sublime text](http://www.sublimetext.com/);

4. Understand the three main stages of git:
![git stages][git-stages-graph]

5. Always remember to keep the shared codebase *(especially `master`)* clean and depolyable;

6.  Do NOT commit any confidential information such as database/server credentials, encryption/decryption keys and etc; Those should be kept either in environment variables or in a key management system like [AWS Key Management Service](http://aws.amazon.com/kms/);

7. Make use of `.gitignore` file to keep any automated artifacts, OS specific files and private files locally;
>[gitignore.io](https://www.gitignore.io/) provides a simple web interface to generate a base `.gitignore` file for different types of project

8. Write proper commit messages in a imperative way to help others understand your work; For example, `Fix bug #1234` instead of `Fixed/Fixes bug #1234`; See more suggestions on http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html;

## Recommend Workflow
a. Fork the project repository and make sure to keep your forked repo synced; Instruction can be found in https://help.github.com/articles/fork-a-repo/;

b. Create a branch on your own forked repo for a new feature or bug fix;

c. Rebase your branch to the `master` of your forked repo *(make sure the `master` branch is synced with the origin)*;

d. Submit a pull request to original project repo after the work has passed through production checks;

## Common Commands

| Command   |      Description       |
|:----------|:-------------|
| `git init` or `git clone <repo url>` | To obtain a git repository |
| `git status` | Show the status of your working directory *(e.g. which files have been modified)*  |
| `git add` | Add files to staging area |
| `git commit` or `git commit -am "your commit message"`| Move files from staging area to local history |
| `git stash` | Save all uncommitted changes and convert back to a clean working directory |
| `git log` | Go through the hisotry of the repository |
| `git checkout -- <filename>` or `git revert <commit>` or `git reset`| Undo changes on a specific file/a certain commit |
|  `git pull` |  == `git fetch` + `git merge` |
| `git branch`, `git checkout`, `git rebase` | Branch Management |
| `git remote add/rename/set-url <remote>` | Remote Management |

For more detail, you may check out the [github git cheatsheet][github-git-cheatsheet].

## How-to


## Reference
[Rangle.io git training](https://github.com/rangle/git-training), [Learn git in 15 minutes](https://try.github.io/levels/1/challenges/1), [Github Help](https://help.github.com/)

[git-logo]: https://git-scm.com/images/logos/2color-lightbg.png
[git-stages-graph]: https://camo.githubusercontent.com/347f01ba29f45507e574916c4cb46550e99919b5/687474703a2f2f6d61726b6c6f6461746f2e6769746875622e696f2f76697375616c2d6769742d67756964652f62617369632d75736167652e7376672e706e67
[github-git-cheatsheet]: https://training.github.com/kit/downloads/github-git-cheat-sheet.pdf
