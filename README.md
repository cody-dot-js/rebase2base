# squash-to
Command line tool to easily squash down your commits to your base branch

## Installation

In your terminal, run the following commands:

```sh
git clone https://github.com/dev-cprice/squash-to.git
cd squash-to
cp squash-to /usr/local/bin/squash-to
```

## Usage

Pass in your base branch as an argument to `squash-to`, which will determine the number of commits since your base branch, and then run `git rebase -i HEAD~NUM_COMMITS_SINCE_BASE_BRANCH`

```sh
# ex: 6 commits since base branch of master
$ squash-to master
#=> will run `git rebase -i HEAD~6
```
