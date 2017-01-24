# ScPo-CompEcon Syllabus

* **Course:** Computational Economics for PhDs
* **Teacher:** Florian Oswald, [florian.oswald@sciencespo.fr](mailto:florian.oswald@sciencespo.fr)
* **Class Times:** Weekly Friday 14:45-16:45 starting 27 of January
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
1. Some experience with the [Unix Shell](https://en.wikipedia.org/wiki/Unix_shell) and the verion control system Git would be very useful - for this course, and for the rest of your life as a scientist. I do therefore recommend that you spend some time with the following excellent tutorials:
    1. [Software Carpentry: The Unix Shell](http://swcarpentry.github.io/shell-novice/): If you have never heard of unix, please go over the first three (very short) chapters:
        * chapters:
            * http://swcarpentry.github.io/shell-novice/01-intro/
            * http://swcarpentry.github.io/shell-novice/02-filedir/
            * http://swcarpentry.github.io/shell-novice/03-create/
        * Where is my Shell Terminal?
            * If you are on Mac OSX, go to Applications, Utilities, Terminal.
            * On Linux, I bet you know.
            * On Windows, you need to make up for the fact that you are not a Unixy system. I recommend [Gnu on Windows (GOW)](https://github.com/bmatzelle/gow/wiki)
    1. [What is Version Control? 5 minute video.](http://git-scm.com/video/what-is-version-control)
        * [Try Git on codeschool.org](https://try.github.io/levels/1/challenges/1): This is a 15 minute intro to Git. So cool!


## Homeworks

There will be homeworks. They will be listed within the [Course Outline](#course-outline).


## Term paper

You are expected to produce a term paper over the course of the semester.  This could be:

* A replication of a paper that uses computational methods.
* Computing additional things that another (maybe theoretical) paper does not compute.
* Ideally, it would be your own research project.


## Textbooks

There are some excellent references for computational methods out there. This course will use material from 

* **Fackler and Miranda** (2002), Applied Computational Economics and Finance, MIT Press
* **Kenneth Judd** (1998), Numerical Methods in Economics, MIT Press
* Nocedal, Jorge, and Stephen J. Wright (2006): Numerical Optimization, Springer-Verlag

(recommended ones in bold face)


## Course Outline

### Introduction, Logistics and Intro to Julia

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

____

### Session: More MPEC Applications

* BLP as an MPEC as in Fox, Dube and Su

____

### Session: Application to Discrete/Continuous Choice in Dynamic models

* Ishkakov, Jorgensen, Rust and Schjerning

___


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
Copyright 2017 Florian Oswald, Sciences Po Paris, florian.oswald@gmail.com
```

Thank you.

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This <span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" rel="dct:type">work</span> and all other materials under https://github.com/ScPo-CompEcon are licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.
