footer: © The Motley Fool, 2014
slidenumbers: true

# Advanced Git

---
## Why Go Beyond Merge?

- The utility of source control is limited by the comprehensibility of the version history
- Ultimately, using advanced git tools is about improving teamwork, collaboration, and communication

---

## Good Commits

---

## Good Commit Messages

---

### Not for You, for Your Coworkers

- You may be unavailable and unreachable (another dimension, dead, etc).
- You may not work here anymore.
- You may forget.

---

### Explain the "Why", not the "What"

- Code and version control already shows *what* you did
- Need to explain business/use case
- Include names of people, dates, etc of justification
- CYA!!

---

### Sample Template

```
Summarize what changes do < 50 chars

More detailed explanation, wrapping at ~72 chars, with an empty line between
the "title" and the "body". Explain motivation for changes, and describe
difference between previous state and current state.
- Optionally with bullet points

```

---

## Local Branches
### Why always working on a branch makes life easier

---

### Branches are cheap!

- Branch entry is just reference to point in time
- Edits on branch recorded as changes from branch point
- Many branches, single working copy.

![inline fill](branch.png)

---

### You'll be prepared!

- Never know how long a change will take
- Working on multiple changes/fixes at the same time
- Emergency work, can be created after the fact, but now you have 2 problems

---

### Easy to keep up-to-date!

- Pull often (rebase or merge, discussed later)
- Easier to deal with lots of small changes/conflicts, if any, daily

---

### Examples

In the beginning:
```sh
$ git checkout master
$ git checkout -b fix-divide-by-zero origin/master  # descriptive branch name!
```

While working:
```sh
$ git pull
```

In the end:
```sh
$ git rebase -i
$ git checkout master
$ git merge -no-ff fix-divide-by-zero
$ git branch -d fix-divide-by-zero
```

---


## Stash

---

### Squirrel!?

- Holding onto uncommitted changes without dirtying history
- Specific to the branch
- Multiple stashes possible, give them names
- Can be turned into branches
- Useful when need to pull latest without committing

---

### Examples

Simplest form
````sh
$ git stash        # or git stash "name of stash"
$ git stash pop
````

Getting latest without committing
````sh
$ git stash && git pull && git stash pop
````

## Love (and Fear) Rebase

---

## Releases

2 Strategies

1. Release Branches
2. Master is Deployable

---

### Release Branches

- New work lands in master
- Each release has a branch
- Specific commits are cherry-picked ("back-ported") into release branches as necessary
- Tags on branches when deployed

---

### Master is Deployable

- New work is done on feature branches
- Feature branches not merged until passing tests and code review
- All deployments come from master

---

### Doesn't matter.  Team needs to pick one and stick to it.

---

## How to Get Out of Trouble

### Dragons Lie Ahead

---

## Putting it all together

### Github Flow

---

Processed used by Github to work on Github

1. Create a branch
1. Add commits
1. Rebase -i
1. Open a Pull Request (or ask for Code Review)
1. Discuss/Review
1. Merge (--no-ff)
1. Deploy

---

## Hands on Workshop

#### If There is Interest

---

## Would you like to play a game?

#### http://pcottle.github.io/learnGitBranching/

---

## Questions?

---
