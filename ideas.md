pro-git book for pictures!

https://github.com/themotleyfool/advance-git-tech-talk

Deckset

1. Commit Messages
	a. Imperative Form
	a. “Why”, not “What”
		- Subject/First Line: Description of changes.
		- Body: Explanation, example, dangers, motivations, etc
	a. Examples
		- Bad - can steal from any one of the repos
		- Good
	a. https://github.com/themotleyfool/financials/wiki/Git-Commit-Guide
1. Local Branches
	a. Branches are cheap!!
	a. Never know how long something will take, just stick it on a branch
	a. Easy to manage multiple items at once, particularly emergencies
	a. Keep up to date - merge vs rebase (pull)
1. Stashing
1. Why to Love and Fear Rebase
	a. how rebase works, and why you should be careful with stuff other people have already seen and/or pulled (maybe with pictures!!!)
		- note that rebases and amends create new commit SHAs (explain why)
	a. rebase -i
		- learn to not care about local history
		- commit often locally - can always get back to the point that USED to work
		- REWRITE - look! I’m a soopah genius
			1. fix, squash, reordering, edit, etc
			1. edit: edit the message, amend the commit, make a fresh commit
		- autosquash?
	a. Careful what you push after a rebase -- you’re gonna have a bad day
1. Release Branches and Tagging vs “master is deployable”
1. How do I Get Out of Trouble? **Dangerzone**
	a. git ref-log
		- Note that ref-log stores local reference info only
	a. git reset vs git reset --hard vs git checkout -- <file>
	a. push w/ force
	a. filter-branch
1. Putting it all together (Github Flow)
	a. Github has dozen of developers working on single project, and all goes pretty okay
	a. local branch for everything
	a. rebase branch against master often
	a. commit often
	a. rebase -i to make logical commits
	a. review with someone (PR if on Github, etc)
	a. merge with -no-ff (99% of time will do this on it’s own)
	a. destroy local branch
1. Separate meeting for practice tutorial or discussion on live implementation in a group




