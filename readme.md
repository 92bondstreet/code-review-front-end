# Code Review Checklist for Front-End Developers


The goal is not to define a formal definition of practices for code review but to give some checklist for reviewers. 

Of course, it helps a developer to know how the reviewer does his code review. He can so focus on writing a better and simpler code.

We speak about because the code author doesn't make his own code review. The developer needs a new way. Of course, the developer could continue to refactor his code to improve it.


## Philosophy


		Code Review is about the code not about the coder.


Basically, the code review focuses only on code written.
 
It's not the time to blame the author but to verify that the code meets the defined standards, best practices... 

It means that no one escapes thec code review: new hire, a senior, the lead developer or even CTO.

**What must be understood is that there is no written well enough to not be seen code.**

This is also the time to share development techniques, tips ... and why not initiate discussions or debate on a particular way of coding.



## Checklist

The checklist is a set of points that are checked during code review. 

So it helps developers to understand what will be reviewed.


### 0. Style and Code Guidelines

In fact, this item is value 0 because it does not fit in the checklist itself: it has to be followed everytime.

It means each developer has to follow the defined Coding Guidelines.

### 1. Code Quality

The code quality allows two things: 

* One, reduce the rate of bugs
* Two, to make the code readable by everyone.
 
The front-end team could use some tools like [JSHint](http://www.jshint.com/) or [Plato](https://github.com/es-analysis/plato) to monitor code quality in JavaScript.
 
 
### 2. Consistency

The reviewer obviously ensures that the written code responds well to the problem of features or defects.


### 3. Simple

The reviewer ensures that the code gets straight to the point. 

We can then help the cyclomatic complexity calculated by JSHint (see point 2). 

There is a correlation between complexity and the likely bugs rate. 

Basically, the more complicated it is, the more simplified.


### 4. Maintenable

The reviewer ensures that another developer can change the code in a small time. 

The code is modular (with pattern, for example) and the variables or methods names are explicit. 

This is true for the CSS or HTML with explicit selectors. We must be able to understand what name the class or method performs. 

It also checks the rule of **One method, one thing**.


### 5. Performance

Performance is not limited to the minification of js or css files and use sprites for images. 

This also happens in loops, array access, DOM access... 

jsPerf is an excellent online tool that allows you to test the performance of a piece of code on different browsers : [http://jsperf.com/](http://jsperf.com/)

Example : [Comparing the performance difference of varied jQuery 1.7 selectors ?](http://jsperf.com/id-vs-class-vs-tag-selectors/2)

## Deep diving

* CodeShip Code Review: [http://blog.codeship.io/2013/08/22/the-codeship-workflow-part-2-pull-requests-and-code-review.html](http://blog.codeship.io/2013/08/22/the-codeship-workflow-part-2-pull-requests-and-code-review.html)

* Code Review with Microsoft tools: [http://msdn.microsoft.com/en-us/library/hh474795.aspx#code_review_request](http://msdn.microsoft.com/en-us/library/hh474795.aspx#code_review_request)

* Checklist example: [http://courses.cs.washington.edu/courses/cse403/12wi/sections/12wi_code_review_checklist.pdf](http://courses.cs.washington.edu/courses/cse403/12wi/sections/12wi_code_review_checklist.pdf)

* Hadoop Code Review: [https://wiki.apache.org/hadoop/CodeReviewChecklist](https://wiki.apache.org/hadoop/CodeReviewChecklist)

## Authors and contributors

### Current
* [Yassine Azzout](http://yass.io) (Creator)

### License
[MIT license](http://www.opensource.org/licenses/Mit)