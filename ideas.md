pro-git book for pictures!

https://github.com/themotleyfool/advance-git-tech-talk

Deckset

1. Commit Messages
  1. Imperative Form
  1. “Why”, not “What”
    - Subject/First Line: Description of changes.
    - Body: Explanation, example, dangers, motivations, etc
  1. Examples
    - Bad - can steal from any one of the repos
    - Good
  1. https://github.com/themotleyfool/financials/wiki/Git-Commit-Guide
1. Local Branches
  1. Branches are cheap!!
  1. Never know how long something will take, just stick it on a branch
  1. Easy to manage multiple items at once, particularly emergencies
  1. Keep up to date - merge vs rebase (pull)
1. Stashing
1. Why to Love and Fear Rebase
  1. how rebase works, and why you should be careful with stuff other people have already seen and/or pulled (maybe with pictures!!!)
    - note that rebases and amends create new commit SHAs (explain why)
  1. rebase -i
    - learn to not care about local history
    - commit often locally - can always get back to the point that USED to work
    - REWRITE - look! I’m a soopah genius
      1. fix, squash, reordering, edit, etc
      1. edit: edit the message, amend the commit, make a fresh commit
    - autosquash?
  1. Careful what you push after a rebase -- you’re gonna have a bad day
1. Release Branches and Tagging vs “master is deployable”
1. How do I Get Out of Trouble? **Dangerzone**
  1. git ref-log
    - Note that ref-log stores local reference info only
  1. git reset vs git reset --hard vs git checkout -- <file>
  1. push w/ force
  1. filter-branch
1. Putting it all together (Github Flow)
  1. Github has dozen of developers working on single project, and all goes pretty okay
  1. local branch for everything
  1. rebase branch against master often
  1. commit often
  1. rebase -i to make logical commits
  1. review with someone (PR if on Github, etc)
  1. merge with -no-ff (99% of time will do this on it’s own)
  1. destroy local branch
1. Separate meeting for practice tutorial or discussion on live implementation in a group
