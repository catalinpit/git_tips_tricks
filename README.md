# GIT TIPS AND TRICKS 🔥🚀⚡

For Git basics visit this link - [Git basics](https://rogerdudler.github.io/git-guide/).

A repo containing only Git tips and tricks.

**`git log -10 --pretty --oneline`**

Displays your last 10 latest commits, each on their line.

`-10` can be replaced with any number you want.

**`git checkout -`**

Jumps back to your last branch.

**`git reflog`**

Displays all the steps you have made

**`git log -s mykeyword`**

Searches through your commits for a commit matching your keyword.

Replace `mykeyword` with the word you want to find

**`git switch -c "new_branch"`**

Did you make the changes in the wrong branch?

This command creates a new branch and moves all your changes to the newly created branch.

**`git switch "branch_name`**

The same as above, but it moves the changes to an existing branch.

**`git log --graph --oneline --decorate --all`**

An ASCII art tree of all the branches, decorated with the names of tags and branches.

**`git commit --amend`**

Edit the **last commit message** and save the commit. If you have already pushed the code, push again by using `--force` flag to make changes to remote repository.

**`git shortlog`**

Summarizes git log output in a format suitable for inclusion in release
announcements. Each commit will be grouped by author and title. ([source](https://git-scm.com/docs/git-shortlog)) ([@natterstefan](https://twitter.com/natterstefan/status/1244888942165610497))

# GIT ALIASES

Create shorter git commands with git aliases.

To add new ones, use the following command `git config --global alias.[insertYourShortcut] [gitCommand]`.

These are mine:

```
git config --global alias.c checkout
git config --global alias.st status
git config --global alias.cm 'checkout master'
git config --global alias.b branch
git config --global alias.c checkout
git config --global alias.ci 'commit -m'
git config --global alias.p pull
git config --global alias.cb 'checkout -b'
git config --global alias.sc 'switch -c'
```

To easily display your git aliases run this command in your terminal - `! git config --get-regexp ^alias\. | sed -e s/^alias\.// -e s/\ /\ =\ /`.

Now you can use `git alias` to list all the aliases you have created.
