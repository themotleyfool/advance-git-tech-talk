footer: © The Motley Fool, 2014
slidernumbers: true

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

- You may not be available and unreachable (another dimension, dead, etc).
- You may not work here anymore.
- You may forget.

---

### Explain the "Why", not the "What"

- Code and version control already shows *what* you did
- Need to explain business/use case
- Include names of people, dates, etc of justification
- CYA!!

---

## Local Branches

---

### Branches are cheap!

- Branch entry is just reference to point in time
- Edits on branch recorded as changes from branch point
- Many branches, single working copy.

---

### Be Prepared!

- Never know how long a change will take
- Working on multiple changes/fixes at the same time
- Emergency work
- Can be created after the fact, but now you have 2 problems

---

### Keeping Up to Date

- Pull often (rebase or merge, discussed later)
- Easier to deal with lots of small changes/conflicts, if any, daily

---

### Examples

In the beginning:
```shell
$ git checkout master
$ git checkout -b fix-divide-by-zero origin/master  # descriptive branch name!
```

While working:
```shell
$ git pull
```

In the end:
```shell
$ git rebase -i
$ git checkout master
$ git merge -no-ff fix-divide-by-zero
$ git branch -d fix-divide-by-zero
```

---


## Stash

---

## Love (and Fear) Rebase

---

## Releases

---

## How to Get Out of Trouble

### Dragons Lie Ahead

---

## Putting it all together

### Github Flow

---

## Hands on Workshop

#### If There is Interest

---

## Questions?

---
