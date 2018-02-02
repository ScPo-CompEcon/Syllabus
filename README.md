# ScPo-CompEcon Syllabus ![](ScPo.png)



* **Course:** Computational Economics for PhDs
* **Teacher:** Florian Oswald, [florian.oswald@sciencespo.fr](mailto:florian.oswald@sciencespo.fr)
* **Class Times:** Thursdays 14:45-16:15
* **Class Location:** Salle J205, 13 rue de l'université
* **Slack**: You have an invitation for our [Slack group](scpo-compecon.slack.com) (ask me for one, if not!)

## Course Description

This is a course for PhD students at the [Department of Economics at Sciences Po](http://econ.sciences-po.fr) in Computational Economics. 

## Course Overview

In this course you will learn about some commonly used methods in Computational Economics. These methods are being used in all fields of Economics. The course has a clear focus on applying what you learn. We will cover the theoretical concepts that underlie each topic, but you should expect a fair amount of *hands on* action required on your behalf. In the words of the great [Che-Lin Su](https://bfi.uchicago.edu/people/che-lin-su):

> Doing Computation is the only way to learn Computation. Doing Computation is the only way to learn Computation. Doing Computation is the only way to learn Computation.

True to that motto, there will be homeworks for you to try out what you learned in class. There will also be a term paper. It will be helpful to bring a laptop to the sessions if you have one.

Topics will be demonstrated through live-code examples/slides, available at [https://scpo-compecon.github.io/CoursePack/](https://scpo-compecon.github.io/CoursePack/).  


## Prerequisites

1. You need a laptop. No programming skills required.
1. You must sign up for a free account at github.com.
1. You must submit your solutions to the [git challenge](challenge.md) by January 31, the day before our first class.

### Getting Programming Skills

1. If you followed Tyler Abbot's **introduction to programming** class last year, you should be all set. If you haven't, or would like a refresher, why not follow **introduction to programming** taught by Hugo Lhuillier this semester (staring January 2018)? I *warmly* recommend to attend this course if you did not sit Tyler's course.
1. We will be using [Julia](http://julialang.org/) for this course. Julia version `1.0` is planned for release early 2018, and depending on that release I will ask you to install a certain version of Julia. Stay tuned. If you have some programming experience in other languages, maybe this is interesting for you:
    - [Noteworthy Differences from Other Languages](https://docs.julialang.org/en/stable/manual/noteworthy-differences/)
    - [MATLAB, Python, Julia Syntax Comparison](http://cheatsheets.quantecon.org/)
1. Hugo in his course will introduce you to things like the [Unix Shell](https://en.wikipedia.org/wiki/Unix_shell) and the verion control system Git. Both of those are very useful - for this course, and for the rest of your life as a scientist. If you want to get a headstart, why not have a peek at those excellent tutorials:
    1. [Software Carpentry: The Unix Shell](http://swcarpentry.github.io/shell-novice/): If you have never heard of unix, please go over the first three (very short) chapters:
        * chapters:
            * http://swcarpentry.github.io/shell-novice/01-intro/
            * http://swcarpentry.github.io/shell-novice/02-filedir/
            * http://swcarpentry.github.io/shell-novice/03-create/
        * Where is my Shell Terminal?
            * If you are on Mac OSX, go to Applications, Utilities, Terminal.
            * On Linux, I bet you know.
            * On Windows, you need to make up for the fact that you are not a Unixy system. I recommend [Gnu on Windows (GOW)](https://github.com/bmatzelle/gow/wiki)
1. [What is Version Control? watch this 5 minute video.](http://git-scm.com/video/what-is-version-control)


## Homeworks

There will be homeworks. They will be listed within the [Course Outline](#course-outline).


## Term Project

This year we will try and implement a prototype for a new course allocation algorithm for SciencesPo students. There was a task force on this last year to work on a solution, and they came up with a workable algorithm. Despite the theory being available, the computational problem to actually **compute** the allocation remains formidable (it will have to make use of distributed computation across many computers in the end). We will have a crack at it. This is a class-wide project to which we are all going to contribute to. Real-world open source software development in your classroom!   
(:wrench:, :muscle:, :tada:) `=>` (acquire the tools, do the work, tada!)

### details

You will work in teams of 2. Details tbc.
  

## Textbooks

There are some excellent references for computational methods out there. This course will use material from 

* **Fackler and Miranda** (2002), Applied Computational Economics and Finance, MIT Press
* **Kenneth Judd** (1998), Numerical Methods in Economics, MIT Press
* Nocedal, Jorge, and Stephen J. Wright (2006): Numerical Optimization, Springer-Verlag

(recommended ones in bold face)


## Course Outline

### Session 1

1. Explain how slides work
1. Talk through homework requirements
1. Talk through term project requirements
1. Basic Computing concepts
    * The fundamental tradeoff: Speed vs Accuracy
    * Some numerical gotchas
    * Computer Basics
    * Intro to `Julia`

#### Reading

* Aruoba and Fernandez-Villaverde (2014) [A Comparison of Programming Languages in Economics](http://economics.sas.upenn.edu/~jesusfv/comparison_languages.pdf)

#### Homework

* [Make a pull request.](https://github.com/ScPo-CompEcon/Students)

___

### Session 2: Continue with Intro to Julia

* Arrays
* Broadcast
* Control Flow
* Types
* Intro to Plots.jl
* Metaprogramming

___


### Session 3: Integration and Function Approximation

1. Numerical Integration
    * Monte-Carlo integration
    * Gaussian Quadrature
    * Multidimensional Quadrature
        * Quadrature with correlated shocks
2. Function Approximation
    * Polynomial Interpolation
        * Basis functions and Coefficients
    * Regression as Approximation
    * Colocation Methods
    * Multidimensional Approximation
        * The Smolyak Grid

___

        
### Session 4: Optimisation 1

1. Intro
2. Conditions for Optima
3. Derivatives and Gradients
4. Numerical Differentiation
5. JuliaOpt

___

### Session 5: Optimisation 2 

1. Bracketing
2. Local Descent
3. First/Second Order and Direct Methods
4. Constraints

___
        

### Session 6: Numerical Dynamic Programming

* Review of DP theory
* Different Solution methods for different cases
    * Discretization
    * Parametric approximation methods [basically Function Approximation](#Function-Approximation)
    * The Endogenous Grid Method
    * Finite time vs inifinite horizon models

___
        

### Session 7: Constrained Optimisation Applications as MPECs

* What is an MPEC?
* How can we cast constrained problems as MPECs?

Applications:

1. MPEC on John Rust's Bus Engine Replacement
1. The Berry-Levinsohn-Pakes (BLP) paper as constrainted optimization problems

___

        
### Session 8: Performant Julia, Parallel Julia and Julia in the Cloud

* Brief intro to parallel computing concepts
* Parallel computing with julia


____

### Session 9: Term Project


____

### Session 10: Term Project


___


## Grading

50% contribution to term project, 50% homeworks

## Statements on Plagiarism

We will try to honour [Science Po's anti-plagiarism policy](http://www.sciencespo.fr/welcome/en/content/plagiarism):

>Plagiarism occurs when a student submits work that does not allow one to distinguish the student's own thoughts from those of other authors: it can be characterised by the absence of citation of a group of consecutive words (five or more), by reformulation or translation, or by copying directly." (article on intellectual honesty)


### Related to Plagiarism

Reuse and building upon ideas or code are major parts of modern software development. As an economist writing code, you will (hopefully) never write anything from scratch. This class is structured such that all solutions are public. You are encouraged to learn from the work of your peers. As I said above, I won't hunt down people who are simply copying-and-pasting solutions, because without challenging themselves, they  are simply wasting their time and money taking this class.

Please respect the terms of use and/or license of any code you find, and if you reimplement or duplicate an algorithm or code from elsewhere, credit the original source with an inline comment.

## License

I took the setup for the structure of this course from [https://github.com/advanced-js](https://github.com/advanced-js) taught by [Aidan Feldman](https://github.com/afeld) and team at NYU, and I would like to thankfully acknowledge making the materials useable to other teachers. The same license applies (below). The coursepack material is based on [Chris Rackauckas' excellent Julia Intro](http://ucidatascienceinitiative.github.io/IntroToJulia/). The license allows you to copy and use everything here, under the condition that you attribute the work (details in the license). The copyright notice to be included in any such copies and other derivative work is:

```
Copyright 2017, 2018 Florian Oswald, Sciences Po Paris, florian.oswald@gmail.com
```

Thank you.

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This <span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" rel="dct:type">work</span> and all other materials under https://github.com/ScPo-CompEcon are licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.
