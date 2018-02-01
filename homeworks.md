### Workflow of Homeworks

The aim of the following setup is to put a system in place by which we can easily look at your solutions to a problem, you can easily look at my solutions (next to yours), and we can also look at the solutions of your peers in order to have a better learning experience. Writing code *is* a activity with tremendous returns from collaboration, and we will try and foster that in this course. Apart from this, a vast amount of high quality code is nowadays developed following this model, so it is a useful skill for you to know how the *fork-change-pull-request model* works. 

If you don't know what Git is, please look at the [prerequisites](#Prerequisites) first.

Here are the overall steps:

1. Fork the repository for homework x (found under [github.com/ScPo-CompEcon](https://github.com/ScPo-CompEcon)). You do that by clicking on *fork* on github.
1. Clone the repository to your computer: use command `git clone https://github.com/your-username/homework-x.git` 
1. Create a new branch on your computer called `my-solution`.
    * you can use the command `git checkout -b my-solution`
1. Modify the files to complete your solution.
1. Make sure your code runs and produces all output.
1. Write some tests for your code if possible.
1. Commit all of your code to your local repository.
1. Push your branch `my-solution` up to your fork of my repo at GitHub.
    * you do `git push origin my-solution` 
1. [Create a pull request for `my-solution`](https://help.github.com/articles/creating-a-pull-request) on the original repository, i.e. the owned by [github.com/ScPo-CompEcon](https://github.com/ScPo-CompEcon). 
1. You can continue to push fixes and improvements until the close date (24 hours before the next class).
1. I will push my solutions to the repository once you have handed in yours. You can then sync your master branch with those solutions. This way, you have both your solutions (on branch `my-solution`) as well as my solution (on the `master` branch).

### Requirements for Homeworks

* I invite you to do the homeworks in teams of 2. 
* You have two weeks for each homework, and they are due 24 hours before the next class, so that I have time to look at them and provide some feedback.
* Please make clear who the contributors are in your comment on the pull request.
* There is clearly a tradeoff between you learning by trying hard, learning from seeing the work of your colleagues, and not learning at all by just copy and pasting the best solution 1 minute before the deadline. I can only remind you that you harm noone but yourself by not exerting effort on the homeworks.
* Each solution you submit must contain text file called `outline.md` where you describe briefly in words what you are doing in your implementation. It is good practice to write this before you even start. (you can always go back and edit this document if you find out that what you wanted to do does not work, but at least you know always what you are trying to do.) 
* Notice the file extension `.md` stands for [`markdown`](https://daringfireball.net/projects/markdown/syntax), probably one of the more amazing inventions of the web. You can super easily generate formated text by just using very intuitive markup symbols. This document is written in markdown.
