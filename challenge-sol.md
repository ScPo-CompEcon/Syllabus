# Github Challenge

## Instructions

You should spend 15 minutes on https://try.github.io/ and then answer the following quiz. You may also find [https://learngitbranching.js.org](https://learngitbranching.js.org) to be fun and helpful to play around with before taking the quiz.

Your answer should be contained in a text file (not .doc) and look something like:

```bash
true
false
false
true
...
```

i.e. there should be one column, and either true or false for each question. Have fun!

## Questions

true		1. `git` is a version control system.
true		1. You can create a git repository anywhere on your computer where you have write access.
false		1. You create an empty git repo by writing `git initiate` in a terminal
true		1. The new file **octocat.txt** being *untracked* means that git sees a new file in this repo.
false		1. If you tell git to `git add octocat.txt`, the file will be saved to an online server.
false		1. If you tell git to `git commit -m 'cool message'`, it will save all files that you staged for commit with `git add` to an online server with the message *cool message* attached.
true		1. If you tell git to `git commit -m 'cool message'`, it will save all files that you staged for commit with `git add` to the repository on your computer with the message *cool message* attached.
true		1. The command `git remote add origin url` associates to your repo an online server called `origin`, that can be reached at the url `url` 
false		1. If you type `git push -u origin master` you get the code from the online server called `origin` onto your computer.
true		1. If you type `git push -u origin master` you send the changes `add`ed to the previous `commit`s to the online server called `origin`.
true		1. saying `git pull origin master` fetches the repo from `origin` and merges it into your local repo.
true		1. After `git pull`ing my collaborators' code from `origin`, `git diff HEAD` shows the difference between my last commit and the latest version on `origin`
true		1. Octocat gets depressed when ocotodog becomes part of the octofamily.
true		1. you can *unstage* a file, i.e. avoid it being included in your next commit by using the `git reset` command.
false		1. In step 1.16 of https://try.github.io/, `git reset` deletes `octofamily/octodog.txt` from your `octofamily` directory.
true		1. creating `branch`es allows you to work on *several verions of your code* before deciding which one to use eventually.
false		1. You create a new branch called `newbranch` with the command `git create branch newbranch`
false		1. You switch to a different branch with `git switch branch`
		1. Suppose you have file `octocat.txt` on the `master branch` and you go through the following sequence of commands:
			* `git branch newbranch`
			* `git checkout newbranch`
			* `git rm octocat.txt`
			* `git commit -m 'removed octocat.txt'`
false			then the file `octocat.txt` has been removed from the `master` branch.
		1. Suppose you have file `octocat.txt` on the `master branch` and you go through the following sequence of commands:
			* `git branch newbranch`
			* `git checkout newbranch`
			* `git rm octocat.txt`
			* `git commit -m 'removed octocat.txt'`
			* `git checkout master`
false			then the file `octocat.txt` has been removed from the `master` branch.
		1. Suppose you have file `octocat.txt` on the `master branch` and you go through the following sequence of commands:
			* `git branch newbranch`
			* `git checkout newbranch`
			* `git rm octocat.txt`
			* `git commit -m 'removed octocat.txt'`
			* `git checkout master`
			* `git merge newbranch`
true			then the file `octocat.txt` has been removed from the `master` branch.