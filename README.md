# ScPo-CompEcon Syllabus ![](ScPo.png)



* **Course:** Computational Economics for PhDs
* **Teacher:** Florian Oswald, [florian.oswald@sciencespo.fr](mailto:florian.oswald@sciencespo.fr)
* **Class Times:** Mondays 10:15-12:15 starting 28 Jan 2019
* **Class Location:** Salle 22, 27 RSG
* **Slack**: I invited you to our [Slack group](https://scpocompecon.slack.com). Please sign up! 

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
2. **Before** you come the first class, please do this:
    1. Download the latest [stable `julia` release (`v1.0.3` as of today)](https://julialang.org/downloads/) for your OS.
    2. Start `julia` by double-clicking on the relevant icon
    3. In the `julia` console:
        1. type `]` (switches into the Package Manager Mode)
        2. type `add IJulia InstantiateFromURL` and hit `Enter`
        3. type `using InstantiateFromURL` and hit `Enter`
        4. type (or copy/paste) `activate_github("QuantEcon/QuantEconLectureAllPackages", tag = "v0.9.5", add_default_environment = true)`. Hitting `Enter` will download a bunch of packages and it will **compile** them for about 10 minutes. Let your computer just run.

### Getting Programming Skills

1. If you followed Hugo L'Huillier's **introduction to programming** class last year, you should be all set. If you haven't, or would like a refresher, why not follow **introduction to programming** taught by Clement Mazet this semester (staring January 2019)? I *warmly* recommend to attend this course if you did not sit Hugo's course.
1. We will be using [Julia](http://julialang.org/) for this course. 
    - [Noteworthy Differences from Other Languages](https://docs.julialang.org/en/stable/manual/noteworthy-differences/)
    - [MATLAB, Python, Julia Syntax Comparison](http://cheatsheets.quantecon.org/)
1. Clement in his course will introduce you to things like the [Unix Shell](https://en.wikipedia.org/wiki/Unix_shell) and the verion control system Git. Both of those are very useful - for this course, and for the rest of your life as a scientist. If you want to get a headstart, why not have a peek at those excellent tutorials:
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

We will try and further develop a prototype for a new course allocation algorithm for SciencesPo students. There was a task force on this 2 years ago to work on a solution, and they came up with a workable algorithm. Last year's `CompEcon` class developed a [prototype implemetnation](https://github.com/ScPo-CompEcon/CourseMatch.jl). This year we will try to complete what we started with last year!  
(:wrench:, :muscle:, :tada:) `=>` (acquire the tools, do the work, tada!)

### details

You will work in teams of 2/3. Details tbc.
  

## Textbooks

There are some excellent references for computational methods out there. This course will use material from 

* **Fackler and Miranda** (2002), Applied Computational Economics and Finance, MIT Press
* **Kenneth Judd** (1998), Numerical Methods in Economics, MIT Press
* **Nocedal, Jorge, and Stephen J. Wright** (2006): Numerical Optimization, Springer-Verlag
* [**Kochenderfer and Wheeler**](https://mitpress.mit.edu/books/algorithms-optimization) (2019), Algorithms for Optimization, MIT Press


## Course Schedule

### 1. Programming languages and why `julia`

1. Talk through homework requirements
1. Talk through term project requirements
1. Show where material is and do first set of slides.
    
#### Homework

* Sign up to github.com.
* Sign up for [introduction to github](https://lab.github.com/githubtraining/introduction-to-github) and send me a screenshot of all completed issues.
* [Make a pull request.](https://github.com/ScPo-CompEcon/Students)

___

### 2. `julia` setup and Getting Started

* Setup environment
* Tools and Editors
* Examples
* Types
* Essentials
* Speed
* Data and Statistical Packages

___


### 3. Integration and Function Approximation

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

### 4. Optimisation 1

1. Intro
2. Conditions for Optima
3. Derivatives and Gradients
4. Numerical Differentiation
5. JuliaOpt

___

### 5. Optimisation 2 

1. Bracketing
2. Local Descent
3. First/Second Order and Direct Methods
4. Constraints

___


### 6. Numerical Dynamic Programming

* Review of DP theory
* Different Solution methods for different cases
    * Discretization
    * Parametric approximation methods [basically Function Approximation](#Function-Approximation)
    * The Endogenous Grid Method
    * Finite time vs inifinite horizon models
+ Solving the Growth Model in 7 Different ways

___


### 7. Constrained Optimisation Applications as MPECs

* What is an MPEC?
* How can we cast constrained problems as MPECs?

Applications:

1. MPEC on John Rust's Bus Engine Replacement
1. The Berry-Levinsohn-Pakes (BLP) paper as constrainted optimization problems

___

        
### 8. HPC `julia`

* Brief intro to parallel computing concepts
* Parallel computing with julia
* GPU computing with julia


____

### 9. Solving the McCall Search Model


____

### 10. Term Project


___

### 11. Term Project


___

### 12. Term Project


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
Copyright 2019 Florian Oswald, Sciences Po Paris, florian.oswald@gmail.com
```

Thank you.

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This <span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" rel="dct:type">work</span> and all other materials under https://github.com/ScPo-CompEcon are licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.
