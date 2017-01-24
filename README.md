# ScPo-CompEcon Syllabus

[![Join the chat at https://gitter.im/ScPo-CompEcon/Syllabus](https://badges.gitter.im/ScPo-CompEcon/Syllabus.svg)](https://gitter.im/ScPo-CompEcon/Syllabus?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)



* **Course:** Computational Economics for PhDs
* **Teacher:** Florian Oswald, [florian.oswald@sciencespo.fr](mailto:florian.oswald@sciencespo.fr)
* **Class Times:** Weekly Friday 14:45-16:45 starting 27 of January, ending 8 of April.
* **Class Location:** Salle : 911 - 9, rue de la chaise
* **Chatroom:** [![Join the chat at https://gitter.im/ScPo-CompEcon/Syllabus](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/ScPo-CompEcon/Syllabus?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

## Course Description

This is a course for PhD students at the [Department of Economics at Sciences Po](http://econ.sciences-po.fr) in Computational Economics. 

## Course Overview

In this course you will learn about some commonly used methods in Computational Economics. These methods are being used in all fields of Economics. The course has a clear focus on applying what you learn. We will cover the theoretical concepts that underlie each topic, but you should expect a fair amount of *hands on* action required on your behalf. In the words of the great [Che-Lin Su](https://bfi.uchicago.edu/people/che-lin-su):

> Doing Computation is the only way to learn Computation. Doing Computation is the only way to learn Computation. Doing Computation is the only way to learn Computation.

True to that motto, there will be homeworks for you to try out what you learned in class. There will also be a term paper. It will be helpful to bring a laptop to the sessions if you have one.

Topics will be demonstrated through live-code examples/slides, available at [ScPo-CompEcon.github.io/slides](http://ScPo-CompEcon.github.io/slides).  


## Prerequisites

1. We will be using [Julia](http://julialang.org/) for this course. Please download the latest stable release [here (v0.5.0)](http://julialang.org/downloads/). Please read in full the following short pieces after you installed the program:
    - [Noteworthy Differences from Other Languages](http://docs.julialang.org/en/release-0.5/manual/noteworthy-differences/)
    - [Performance Tips](http://docs.julialang.org/en/release-0.5/manual/performance-tips/)
    - [MATLAB, Python, Julia Syntax Comparison](http://cheatsheets.quantecon.org/)
1. Some basic programming experience in julia, R, python, C++, java, fortran, etc. would be helpful. [Stata doesn't count.] You must know and be able to work with the terms *variable*, *memory*, *loop* and *array*.
    1. A good place to start with Julia is the [quant-econ.net website](http://quant-econ.net/jl/learning_julia.html)
    1. Otherwise it may be useful to go through a short Python tutorial. Once you know a bit of Python, `Julia` will be very close:
        * [http://www.learnpython.org](http://www.learnpython.org)
        * [http://www.trypython.org](http://www.trypython.org)
    1. There are more tutorials listed below in subsection [Julia tutorials](#julia-tutorials)
1. Some experience with the [Unix Shell](https://en.wikipedia.org/wiki/Unix_shell) and the verion control system Git would be very useful - for this course, and for the rest of your life as a scientist. I do therefore recommend that you spend some time (2h total max) with the following excellent tutorials:
    1. [Software Carpentry: The Unix Shell](http://swcarpentry.github.io/shell-novice/)
        * If you are on MacOS/Unix, just open the terminal application and you're good to go.
        * On Windows, you need to make up for the fact that you are not Unix. I recommend [Gnu on Windows (GOW)](https://github.com/bmatzelle/gow/wiki)
    1. [What is Version Control? 5 minute video.](http://git-scm.com/video/what-is-version-control)
        * [Try Git on codeschool.org](https://try.github.io/levels/1/challenges/1): This is a 15 minute intro to Git. So cool!


## Homeworks

Each session is accompagnied by a homework. They will be listed within the [Course Outline](#course-outline).

### Workflow of Homeworks

The aim of the following setup is to put a system in place by which we can easily look at your solutions to a problem, you can easily look at my solutions (next to yours), and we can also look at the solutions of your peers in order to have a better learning experience. Writing code *is* a activity with tremendous returns from collaboration, and we will try and foster that in this course. Apart from this, a vast amount of high quality code is nowadays developed following this model, so it is a useful skill for you to know how the *fork-change-pull-request model* works. 

If you don't know what Git is, please look at the [prerequisites](#Prerequisites) first.

If you're using GitHub Desktop, [these instructions](https://help.github.com/desktop/guides/contributing/) will help explain the Git/GitHub concepts. Here are the overall steps:

1. Fork the repository for homework x (found under [github.com/ScPo-CompEcon](https://github.com/ScPo-CompEcon)). You do that by clicking on *fork* on github.
1. Clone the repository to your computer: use command `git clone https://github.com/your-username/homework-x.git` or do in your GUI.
1. Create a new branch on your computer called `my-solution`.
    * you can use the command `git checkout -b my-solution`
1. Modify the files to complete your solution.
1. Make sure your code runs and produces all output.
1. Write a test for your code if possible.
1. Commit all of your code to your local repository.
1. Push your branch `my-solution` up to your fork of my repo at GitHub.
    * you do `git push origin my-solution` 
1. [Create a pull request for `my-solution`](https://help.github.com/articles/creating-a-pull-request) on the original repository, i.e. the owned by [github.com/ScPo-CompEcon](https://github.com/ScPo-CompEcon). 
1. You can continue to push fixes and improvements until the close date (24 hours before the next class).
1. I will push my solutions to Exercise repository once you have handed in yours. You can then sync your master branch with those solutions. This way, you have both your solutions (on branch `my-solution`) as well as my solution (on the `master` branch).

### Requirements for Homeworks

* I invite you to do the homeworks in teams of 2. 
* You have two weeks for each homework, and they are due 24 hours before the next class, so that I have time to look at them and provide some feedback.
* Please make clear who the contributors are in your comment on the pull request.
* There is clearly a tradeoff between you learning by trying hard, learning from seeing the work of your colleagues, and not learning at all by just copy and pasting the best solution 1 minute before the deadline. I can only remind you that you harm noone but yourself by not exerting effort on the homeworks.
* Each solution you submit must contain text file called `outline.md` where you describe briefly in words what you are doing in your implementation. It is good practice to write this before you even start. (you can always go back and edit this document if you find out that what you wanted to do does not work, but at least you know always what you are trying to do.) 
* Notice the file extension `.md` stands for [`markdown`](https://daringfireball.net/projects/markdown/syntax), probably one of the more amazing inventions of the web. You can super easily generate formated text by just using very intuitive markup symbols. This document is written in markdown.

## Term paper

You are expected to produce a term paper over the course of the semester.  This could be:

* A replication of a paper that uses computational methods.
* Computing additional things that another (maybe theoretical) paper does not compute.
* Ideally, it would be your own research project.

### Requirements for the Term paper

* **Due Date**: May 9th 2016.
* You must do this on your own.
* The paper should be *max* 15 pages of double-spaced 12pt font text, excluding any graphs or tables.
* The paper should contain
    1. A motivation/introduction and formulation of the research question.
    2. A justification for why one needs computational methods to answer this question.
    3. A model.
    4. A clear outline describing the computational approach to compute the model.
    5. A presentation of the results.
    6. A discussion of the accuracy of the obtained results.
* Furthermore, the code you write needs to be on github, if you want in a private rather than public repository, to which you grant me access. (you get access to 5 private repos for free). There will be extra marks for code readability and code quality.

### Julia Tutorials

* [quant-econ.net website](http://quant-econ.net/jl/learning_julia.html)
* See at the bottom of the [Julia Manual Introduction](http://docs.julialang.org/en/release-0.4/manual/getting-started/)
* See the [Learning Section](http://julialang.org/learning/) of the Julia homepage.

### Julia Environments

* You can use pure Julia together with a text editor.
    * [sublime text](http://www.sublimetext.com) is a good choice, [http://www.vim.org](http://www.vim.org) if you are hard-core.
    * You can use an IDE (like matlab or RStudio). [Juno](http://junolab.org) is great.

## Textbooks

There are some excellent references for computational methods out there. This course will use material from 

* **Fackler and Miranda** (2002), Applied Computational Economics and Finance, MIT Press
* **Kenneth Judd** (1998), Numerical Methods in Economics, MIT Press
* Nocedal, Jorge, and Stephen J. Wright (2006): Numerical Optimization, Springer-Verlag

(recommended ones in bold face)


## Course Outline

Each subsection here stands for one session of 2 hours. There are 6 subsections.

### First Session: Introduction, Logistics and Numerical Integration

1. Setup
    * How many people are comfortable with Git/GitHub?
    * Install [GitHub Desktop](https://desktop.github.com/)
        * If you are comfortable with Git already, you can skip this.
    * Sign up for GitHub
1. GitHub workflow
    * Walk through [workflow](#workflow)
    * Create pull request on [students repository](https://github.com/ScPo-CompEcon/students)
1. Explain how slides work
1. Talk through [homework requirements](#homework-projects/requirements)
1. Talk through [term paper requirements](#term-paper/requirements)
1. Talk through [weapon of choice](#weapon-of-choice)

#### Talk about Computation!
1. Basic Computing concepts
    * The fundamental tradeoff: Speed vs Accuracy
    * Some numerical gotchas
    * Computer Basics
    * Intro to `Julia`

#### Reading

* Aruoba and Fernandez-Villaverde (2014) [A Comparison of Programming Languages in Economics](http://economics.sas.upenn.edu/~jesusfv/comparison_languages.pdf)


#### Homework

1. make sure you signed up on github (and put a picture there!)
1. Join [the chat room](https://gitter.im/ScPo-CompEcon). You can ask any question you want there - will see them even if offline.
1. [10 min read] Do this short online tutorial on an [example github workflow](https://guides.github.com/activities/hello-world)
1. [4 min read] Do this short online tutorial on [forking on github](https://guides.github.com/activities/forking/)
1. download [GitHub Desktop](https://desktop.github.com/). [Someone said they are running MacOS < 10.9, and the latest release was 16 years ago. I can't believe that is the case, but please contact me if you cannot install this program.] 
    * Please go through the initial tutorial. It is helpful.
1. do the fork-and-pull-request exercise on the [students repository](https://github.com/ScPo-CompEcon/students)
1. Please note: I added a comment (about a comment) to my `JSON` example file. Make sure your file has exactly that format, and is exactly saved in that location. (you have to look at my repo, not your fork)
___


### Session: Integration and Function Approximation

1. Numerical Integration and Derivation
    * Monte-Carlo integration
    * Gaussian Quadrature
    * Multidimensional Quadrature
        * Quadrature with correlated shocks
    * Numerical Differentiation
        * Finite Differences
        * Automatic Differentiation
        * [JuliaOpt/JuMP.jl](https://github.com/JuliaOpt/JuMP.jl)
2. Function Approximation
    * Polynomial Interpolation
        * Basis functions and Coefficients
    * Regression as Approximation
    * Colocation Methods
    * Multidimensional Approximation
        * The Smolyak Grid


#### Homework

* Fork the homework at [github.com/ScPo-CompEcon/HW-integration](https://github.com/ScPo-CompEcon/HW-integration)
    * Follow steps detailed there.
* Create a new repository on github for your term paper. 
    * Choose a name, whether public of private and select the option to create a README.md file. clone.
    * In the README.md file detail your project idea in a few words (more than 100 but less than 500). If you need math, include an IJulia notebook.
    * If you decide to make this a private repository, you need to add me as a collaborator.
    * push to github.
    * email me the URL of the repo by the homework deadline (24h prior to next class.)

___

        
### Session: Optimisation
1. Unconstrained Optimisation
    * Comparison Methods
    * Newton's Method
    * Line Search, Trust Region, and other Methods
    * Application: Maximum Likelihood
    * Introduce [http://www.juliaopt.org](http://www.juliaopt.org)
1. Constrained Optimization
    * Theory
    * Some Numerical Methods for Constrained Optimization

#### Homework

___

        

### Session: Constrained Optimisation Applications
1. MPEC on John Rust's Bus Engine Replacement
1. The Berry-Levinsohn-Pakes (BLP) paper as constrainted optimization problems


#### Homework

___

        

### Session: Numerical Dynamic Programming

* Review of DP theory
* Different Solution methods for different cases
    * Discretization
    * Parametric approximation methods [basically Function Approximation](#Function-Approximation)
    * The Endogenous Grid Method
    * Finite time vs inifinite horizon models

#### Homework

___

        
### Session: Sky's the Limit - Parallel Computing in the Cloud

* Brief intro to parallel computing concepts
* Parallel computing with julia
* (Free) Cloud computing via the [Github Student Developer Pack](https://education.github.com/pack/join)

#### Homework

___

        

## Pairing Tips

* Three people is possible, but two works best
* Agree on an editor and environment that you're both comfortable with
* The person who's less experienced/comfortable should have more keyboard time
* Switch who's "driving" regularly
* Make sure to save the code and send it to both people

## Resources

### Beginner Materials

### Recommended Reading

### Tools

#### GitHub

* Git and GitHub
    * [Official GitHub Help](https://help.github.com/)
    * [Recommended resources](http://hackerhours.org/resources.html#github)
* GitHub Pages
    * [Official site](http://pages.github.com/)
    * [Thinkful guide](http://www.thinkful.com/learn/a-guide-to-using-github-pages/)



## Grading

50% homeworks, 50% paper

## Statements on Plagiarism

We will try to honour [Science Po's anti-plagiarism policy](http://www.sciencespo.fr/welcome/en/content/plagiarism):

>Plagiarism occurs when a student submits work that does not allow one to distinguish the student's own thoughts from those of other authors: it can be characterised by the absence of citation of a group of consecutive words (five or more), by reformulation or translation, or by copying directly." (article on intellectual honesty)


### Related to Plagiarism

Reuse and building upon ideas or code are major parts of modern software development. As an economist writing code, you will (hopefully) never write anything from scratch. This class is structured such that all solutions are public. You are encouraged to learn from the work of your peers. As I said above, I won't hunt down people who are simply copying-and-pasting solutions, because without challenging themselves, they  are simply wasting their time and money taking this class.

Please respect the terms of use and/or license of any code you find, and if you reimplement or duplicate an algorithm or code from elsewhere, credit the original source with an inline comment.

## License

In setting up this course I was heavily influenced - and shamelessly copied entire parts of - [https://github.com/advanced-js](https://github.com/advanced-js) taught by [Aidan Feldman](https://github.com/afeld) and team at NYU, and I would like to thankfully acknowledge making the materials useable to other teachers. The same license applies (below). The license allows you to copy and use everything here, under the condition that you attribute the work (details in the license). The copyright notice to be included in any such copies and other derivative work is:

```
Copyright 2015 Florian Oswald, Sciences Po Paris, florian.oswald@gmail.com
```

Thank you.

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This <span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" rel="dct:type">work</span> and all other materials under https://github.com/ScPo-CompEcon are licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.
