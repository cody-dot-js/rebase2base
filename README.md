# rebase2base
Command line tool to quickly rebase to your base branch by the number of commits since you branched.

## Installation

In your terminal, run the following commands:

```sh
git clone https://github.com/dev-cprice/rebase2base.git
cd rebase2base
cp rebase2base /usr/local/bin/rebase2base
```

## Usage

Pass in your base branch as an argument to `rebase2base`, which will determine the number of commits since your base branch, and then run `git rebase -i HEAD~NUM_COMMITS_SINCE_BASE_BRANCH`

```sh
# ex: 6 commits since base branch of master
$ rebase2base master
#=> will run `git rebase -i HEAD~6
```
