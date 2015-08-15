![Git](https://git-scm.com/images/logos/2color-lightbg.png)
====

1. You can download it in the following website: https://git-scm.com or you can install it through `brew` if you are using mac computers;

2. Useful gui clients for git repo management:
    >- Mac OSX: [GitX](http://gitx.frim.nl/) (free), [Tower](http://www.git-tower.com/) (commerical);

    >- Window: [GitHub for Windows](https://windows.github.com/), [SmartGit](http://www.syntevo.com/smartgit/)

3. [Git](https://github.com/kemayo/sublime-text-git) and [Git Gutter](https://github.com/jisaacks/GitGutter) packages are good to have if you are using [sublime text](http://www.sublimetext.com/);

4. **Rule #1:** Always remember to keep the shared codebase especially `master` clean and depolyable;

5. **Rule #2:** Do NOT commit any confidential information such as database/server credentials, encryption/decryption keys and etc; Those should be kept either in environment variables or in a key management system like [AWS Key Management Service](http://aws.amazon.com/kms/);

6. Make use of `.gitignore` file to keep any automated artifacts, OS specific files and private files locally;
>[gitignore.io](https://www.gitignore.io/) provides a simple web interface to generate a base `.gitignore` file for different types of project

7. **Rule #3:** Write proper commit messages in a imperative way to help others understand your work; For example, `Fix bug #1234` instead of `Fixed/Fixes bug #1234`; See more suggestions on http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html;

8. Recommend workflow
    >- Fork the project repository and make sure to keep your forked repo synced; Instruction can be found in https://help.github.com/articles/fork-a-repo/;

    >- Create a branch on your own forked repo for a new feature or bug fix;

    >- Rebase your branch to the `master` of your forked repo *(make sure the `master` branch is synced with the origin)*;

    >- Submit a pull request to original project repo after the work has passed through production checks;

9. Common commands
    >- Initiate a git repository: `git init/clone`

    >- File staging: `git add/rm/mv`

    >- Commit work to cloud: `git commit/push`

    >- Branch management: `git branch/checkout/rebase`

    >- Fetch work from the cloud: `git fetch/pull`

    >- Remote management: `git remote add/rm`

10. Reference: [Rangle.io git training](https://github.com/rangle/git-training), [Learn git in 15 minutes](https://try.github.io/levels/1/challenges/1)
