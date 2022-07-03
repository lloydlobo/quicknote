---
id: 4nbo4cbcvioulri6o0q1esm
title: Learnable Programming
desc: ''
updated: 1656827615827
created: 1656821970058
---

Source: <http://worrydream.com/LearnableProgramming/>

## Inspiration

> Designing a programming system for understanding programs - Bret Victor / September 2012

### Contents

> The environment should allow the learner to:
>
> read the vocabulary -- what do these words mean?
> follow the flow -- what happens when?
> see the state -- what is the computer thinking?
> create by reacting -- start somewhere, then sculpt
> create by abstracting -- start concrete, then generalize
> The language should provide:
>
> identity and metaphor -- how can I relate the computer's world to my own?
> decomposition -- how do I break down my thoughts into mind-sized pieces?
> recomposition -- how do I glue pieces together?
> readability -- what do these words mean?- [Inspiration](#inspiration)

## Table of Contents

- [Inspiration](#inspiration)
  - [Contents](#contents)
- [Table of Contents](#table-of-contents)
  - [The features are not the point](#the-features-are-not-the-point)
  - [Read the vocabulary](#read-the-vocabulary)
    - [Make meaning transparent](#make-meaning-transparent)
    - [Explain in context](#explain-in-context)
    - [Summary — Read the vocabulary](#summary--read-the-vocabulary)
  - [Follow the flow](#follow-the-flow)
    - [Make flow tangible](#make-flow-tangible)
    - [Make flow visible](#make-flow-visible)
    - [Make time tangible](#make-time-tangible)
    - [Make time visible](#make-time-visible)
    - [Summary — Follow the flow](#summary--follow-the-flow)
  - [See the state](#see-the-state)
    - [Show the state](#show-the-state)
    - [Show comparisons](#show-comparisons)
    - [Eliminate hidden state](#eliminate-hidden-state)
  - [Create by reacting](#create-by-reacting)
    - [Get something on the screen as soon as possible](#get-something-on-the-screen-as-soon-as-possible)
    - [Dump the parts bucket onto the floor](#dump-the-parts-bucket-onto-the-floor)
    - [Summary — Create by reacting](#summary--create-by-reacting)
  - [Create by abstracting](#create-by-abstracting)
    - [Start constant, then vary](#start-constant-then-vary)
    - [Start with one, then make many](#start-with-one-then-make-many)
    - [Summary — Create by abstracting](#summary--create-by-abstracting)
  - [Language](#language)
    - [Great works](#great-works)
    - [Identity and metaphor](#identity-and-metaphor)
    - [Decomposition](#decomposition)
    - [Recomposition](#recomposition)
    - [Readability](#readability)
- [Summary](#summary)
  - [These are not training wheels](#these-are-not-training-wheels)
- [Relevent Resources](#relevent-resources)

### The features are not the point

> Likewise, a well-designed system is not simply a bag of features.
> >
> A good system is designed to encourage particular ways of thinking,
> with all features carefully and cohesively designed around that purpose.

### Read the vocabulary

![](http://worrydream.com/LearnableProgramming/Images/Vocab2.png)
> Thought experiment. Imagine if you bought a new microwave, took it out of the box, and found a panel of unlabeled buttons.

> Imagine if the microwave encouraged you to randomly hit buttons until you figured out what they did.

![](http://worrydream.com/LearnableProgramming/Images/Vocab5.png)

#### Make meaning transparent

![](http://worrydream.com/LearnableProgramming/Images/Vocab7.png)

![](/assets/images/2022-07-03-10-14-00.png)

#### Explain in context

> One attribute of great explanations is that they are often embedded in the context of what they are explaining.

![](http://worrydream.com/LearnableProgramming/Images/Vocab11.png)

![](/assets/images/2022-07-03-10-15-41.png)

#### Summary — Read the vocabulary

> enabling the learner to read the program.
>
> - The environment should **make meaning transparent**, so the learner can concentrate on high-level concepts, not vocabulary.
> - The environment should **explain in context**. Show and tell. Annotate the data, not just the code.

![](http://worrydream.com/LearnableProgramming/Images/Vocab2.png)
> An environment which allows learners to get hung up on these questions is an environment which discourages learners from even getting started.

### Follow the flow

> A typical live-coding environment presents the learner with code on the left, and the output of the code on the right. When the code is changed, the output updates instantaneously.
>
> ![](http://worrydream.com/LearnableProgramming/Images/Flow1.png)
>
> > Imagine a cooking show, ruthlessly abbreviated.
>![](http://worrydream.com/LearnableProgramming/Images/Flow2.jpg)
>> Of course not. You need to see how the ingredients are combined. You need to see the steps.

> People **understand things that they can see and touch** (and reflect?). In order for a learner to understand what the program is actually doing, the program flow must be made visible and tangible.

#### Make flow tangible

> The "for" construct, with its three statements on a single line, makes the control flow jump around bizarrely, and is an unnecessarily steep introduction to the concept of looping.
> > ![](http://worrydream.com/LearnableProgramming/Images/Flow3.png)
> To make the flow more sane for a learner, the loop can be rewritten using "while":
> > ![](http://worrydream.com/LearnableProgramming/Images/Flow4.png)

> Now, the control flow must be made tangible. We must put the execution of the program into the programmer's hand, let her feel that it is a real thing, let her own it.
> > ![](/assets/images/2022-07-03-10-23-40.png)
> > This control allows the programmer to move around the loop at her **own pace, and understand what is happening at each step**.
> > She can go backwards and forwards, dwell in difficult areas, and compare what is happening at different times.
> > She can study how the output is built up over time, instead of seeing it magically appear all at once.

#### Make flow visible

> follow the program's execution over time. But she's peeking through a pinhole, **only seeing a single point in time at any instant**.
> **She has no visual context.**
> ![](http://worrydream.com/LearnableProgramming/Images/Flow6.png)
>
> Example - the program flow is plotted on a timeline. Each line of code that is executed leaves a dot behind. The programmer can take in the entire flow at a glance:
> >![](/assets/images/2022-07-03-10-27-23.png)
> allows the programmer to see the "shape" of an algorithm, and understand it at a higher level. The program flow is no longer "one line after another", but a pattern of lines over time.
> >![](/assets/images/2022-07-03-10-29-00.png)

#### Make time tangible

> This control enables the programmer to go backwards and forwards through time, study interesting frames, and compare the execution across different frames.

<iframe src="http://worrydream.com/LearnableProgramming/Movies/Flow10.mp4">

#### Make time visible

> all frames are lightly overlaid, in order to give context to the active frame. The entire path of the ball can be seen at once.

<iframe src="http://worrydream.com/LearnableProgramming/Movies/Flow11.mp4" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen>
.

> The output of the program is no longer a series of fleeting moments, but can be seen as a single, solid thing that extends over time. There is great power in this way of thinking.

#### Summary — Follow the flow

> - The environment can make flow tangible, by enabling the programmer to explore forward and backward at her own pace.
> - The environment can make flow visible, by visualizing the pattern of execution.
> - The environment can represent time at multiple granularities, such as frames or event responses, to enable exploration across these meaningful chunks of execution.

### See the state

> The entire purpose of code is to manipulate data, and we never see the data.
> Show the data.
> If you are serious about creating a programming environment for learning, the number one thing you can do -- more important than live coding or adjustable constants, narrated lessons or discussion forums, badges or points or ultra-points or anything else -- is to show the data.

#### Show the state

> Because the value of a variable varies over time, showing the data is intimately connected with showing time.

> it is easy to answer the first two questions. By skimming over the execution of that line of code, we can see all of the values that scaleFactor takes on, and when.

> However, it is still difficult to answer the third question: how does the variable vary? What is the shape of its change? The question is difficult because we are, once again, peeking through a pinhole, only seeing a single point at a time.

> Edward Tufte has a second rule. It is not enough to just show the data. We must show comparisons.

<iframe src="http://worrydream.com/LearnableProgramming/Movies/State3.mp4">

.

#### Show comparisons

> Data needs context. It is rarely enough to see a single data point in isolation
> as the programmer zooms the timeline out, the visualization automatically switches from a table to a plot.

<iframe src="http://worrydream.com/LearnableProgramming/Movies/State9.mp4" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen></iframe>

#### Eliminate hidden state

<iframe src="http://worrydream.com/LearnableProgramming/Movies/State10.mp4"></iframe>

> the learner must see its effect
>
> For example, as the programmer moves over iterations of the "triangle" line, she sees each triangle appear on the canvas:

### Create by reacting

#### Get something on the screen as soon as possible

#### Dump the parts bucket onto the floor

#### Summary — Create by reacting

> The create-by-reacting way of thinking could be stated as: start with something, then adjust until it's right
>
> this does not relieve the programmer from thinking! It simply makes those **thoughts immediately visible.** I am happy to be composing this essay in a text editor, where my words become visible and editable as soon as I think of them, as opposed to working entirely internally like the orators and playwrights of the distant past.
>
> - The environment must be designed to get something on the screen as soon as possible, so the programmer can start reacting. This requires modeling the programmer's thought process, and designing a system that can pick up on the earliest possible seed of thought.
> - The environment must dump the parts bucket onto the floor, allowing the programmer to continuously react to her raw material and spark new ideas.

### Create by abstracting

#### Start constant, then vary

> by providing meaningful ways of gradually and seamlessly transitioning constant expressions into variable expressions.
>
> Here, the programmer selects one of the numbers, and converts it into a variable.

> <iframe src="http://worrydream.com/LearnableProgramming/Movies/Abstract4.mp4"></iframe>
>
> She then connects the variable to another number, by dragging from one to the other.
> <iframe src="http://worrydream.com/LearnableProgramming/Movies/Abstract5.mp4"></iframe>
>
> There are two additional arguments to "triangle" which need to vary as well. When she connects the variable, whose value is 80, to the constant 100, the environment offers a choice of four possible relationships between the numbers.
><iframe src="http://worrydream.com/LearnableProgramming/Movies/Abstract6.mp4"></iframe>
>
> The four expressions involve addition, subtraction, multiplication, and division respectively. One of them will typically be either the correct relationship or a good starting point.
> <iframe src="http://worrydream.com/LearnableProgramming/Movies/Abstract7.mp4"></iframe>
>

#### Start with one, then make many

> by providing ways of using those variable expressions at a higher level, such as function application or looping.
>
> In the following example, the programmer wants to draw a row of houses. She selects the abstracted code, and converts it into a loop.
> Instead of drawing an evenly-spaced row of houses, the programmer now wants individual control over each of the houses. Starting from the variable abstraction, she selects the code and converts it into a function.
> Now, instead of identical houses, she wants to vary the heights of the houses. She introduces another variable, and then converts it into an additional argument to the function.

> <iframe src="http://worrydream.com/LearnableProgramming/Movies/Abstract10.mp4"></iframe>
>
> The process, again, consists of starting concrete, and progressively introducing abstraction:*
<http://worrydream.com/LadderOfAbstraction>
>
> - The programmer creates a drawing of a house.
> >
> > - She turns x into a variable, so she can control the house's position.
> > - She turns x into a function argument, so different houses can have different positions.
> > - She turns y into a variable, so she can control the house's height.
> > - She turns y into a function argument, so different houses can have different heights.
> > - Summary — Create by abstracting
  >  
#### Summary — Create by abstracting

> The learner always gets the experience of interactively controlling the lower-level details, understanding them, developing trust in them, before handing off that control to an abstraction and moving to a higher level of control.
>
> Start concrete, start grounded. Start with one specific case, entirely understood. Then gradually generalize, level by level, in such a way that the programmer still fully understands the program at each level of abstraction.
> >
> Fully concrete code can be micromanaged -- the programmer has explicit control over every step of the execution. Abstraction means giving up some of this control, and this can be scary for a learner.

### Language

> A programming system has two parts. The environment is installed on the computer,
> and the language is installed in the programmer's head.

#### Great works

> ![](http://worrydream.com/LearnableProgramming/Images/Language2.png)
> The canonical work on designing programming systems for learning,
> and perhaps the greatest book ever written on learning in general,
> is Seymour Papert's "Mindstorms".
> >
> [Mindstorms](http://www.amazon.com/dp/0465046746) Amazon
> Mindstorms at [Powell's](http://www.powells.com/biblio/72-9780465046744-0)
> In his influential essay [No Silver Bullet](http://worrydream.com/refs/Brooks-NoSilverBullet.pdf),
> > Fred Brooks makes the case that software is inherently "invisible and unvisualizable",
> > and points out the universal failure of so-called "visual programming" environments.  
> > I don't fault Fred Brooks for his mistake -- the visual programming that
> > he's thinking of indeed has little to offer.  
> > But that's because it visualizes the wrong thing.
> Traditional visual environments visualize the code.  They visualize static structure.
> > But that's not what we need to understand.  We need to understand what the code is doing.
> Visualize data, not code.  Dynamic behavior, not static structure.
> > Maybe we don't need a silver bullet.  
> > > We just need to take off our blindfolds to see where we're firing.

#### Identity and metaphor

> In Logo, the programmer draws pictures by directing the "turtle", an onscreen character which leaves a trail as it moves:
> ![](http://worrydream.com/LearnableProgramming/Images/Language3.png)

#### Decomposition

> This is Alan Kay inventing objects:
> > Bob Barton \[said\] "The basic principle of recursive design is to make the parts have the same power as the whole." For the first time I thought of the whole as the entire computer, and wondered why anyone would want to divide it up into weaker things called data structures and procedures. Why not divide it up into little computers... Why not thousands of them, each simulating a useful structure?

> . In his wonderful essay [Why Functional Programming Matters](http://worrydream.com/refs/Hughes-WhyFunctionalProgrammingMatters.pdf), John Hughes argues that decomposition lies at the heart of the power of languages like Haskell:
> >
> > - When writing a modular program to solve a problem, one first divides the problem into subproblems, then solves the subproblems, and finally combines the solutions. The ways in which one can divide up the original problem depend directly on the ways in which one can glue solutions together. Therefore, to increase one's ability to modularize a problem conceptually, one must provide new kinds of glue in the programming language.
> > - Functional languages provide two new, very important kinds of glue... This is the key to functional programming’s power -- it allows improved modularization.

> A language that discourages decomposition is a language that cripples a programmer's most valuable way of thinking.

#### Recomposition

> A programming language must encourage recomposition -- grabbing parts of other programs, assembling them together, modifying them, building on top of them. This gives creators the initial material they need to create by reacting, instead of facing every new idea with a blank page. It also allows creators to learn from each other, instead of deriving techniques and style in a vacuum.

> Designing a system that supports recomposition demands long and careful thought, and design decisions that make programming more convenient for individuals may be detrimental to social creation.

> Trick question -- it's impossible to know what color it is, because the meaning of "255" depends on the global "color mode". It could be any of these colors:
> ![](http://worrydream.com/LearnableProgramming/Images/Language9.png)

> If two Processing programs specify their colors in different color modes, then combining the two programs is almost hopeless.

#### Readability

> A learner must be able to look at a line of code and know what it means.

> Syntax matters. Here are two statements in HyperCard's scripting language, and their equivalents in a more conventional syntax:

> HyperTalk:
>
> - Write "hello" to file "greetings".
> - Drag from "0,0" to "100,100" with optionKey.
>
> C-like syntax:
>
> - writeFile("hello", "greetings");
> - dragMouse(0, 0, 100, 100, OPTION_KEY);

> As another example, here's how a programmer might draw an ellipse in three languages:
> > Smalltalk: canvas drawEllipseCenteredAtX:50 y:50 width:100 height:100.
> >
> > Processing: ellipse(50,50,100,100);
> >
> > x86 assembly: push 100; push 100; push 50; push 50; call _ellipse

> **Names matter**. Below are four array methods from Apple's Cocoa framework, and the equivalent JavaScript methods:
>> Cocoa: addObject addObjectsFromArray arrayByAddingObject arrayByAddingObjectsFromArray
>>
>> JavaScript: push splice concat concat

## Summary

> The design principles presented in this essay can be used as a checklist to evaluate a programming system for learning.
>
> - Does the environment allow the learner to...
> >
> > - read the vocabulary? -- Is meaning transparent? Is meaning explained in context, by showing and telling?
> > - follow the flow? -- Is time visible and tangible? At all meaningful granularities?
> > - see the state? -- Does the environment show the data? Show comparisons? Is hidden state eliminated?
> > - create by reacting? -- Is something on screen as soon as possible? Is the parts bucket on the floor?
> > - create by abstracting? -- Can the programmer start concrete, then generalize?
>
> - Does the language provide...
> >
> > - identity and metaphor? -- Is the computer's world connected to the programmer's world?
> > - decomposition? -- Can the programmer break down her thoughts into mind-sized pieces?
> > - recomposition? -- Can the programmer put diverse pieces together?
> > - readability? -- Is meaning transparent?
> > - This essay suggested some features and references that address these questions, but the questions matter more than my answers.
>
> > - Some people will defend poorly-designed systems by pointing out all the creativity that they have enabled. For example, if novices are creating lots of programs in the Khan Academy and Processing systems, doesn't that mean the systems are worthwhile and valuable?
> >
> > - Not necessarily. People are inherently creative, and some will manage to create in even the most hostile of environments. That doesn't justify bad design. Ian Bogost has a particularly memorable response to that line of thinking.
> >
> > - If you are designing a system and you can't answer these questions, it's time to reopen your sketchbook, because your design's not done yet.

### These are not training wheels

> A frequent question about the sort of techniques presented here is, "How does this scale to real-world programming?"**This is a reasonable question, but it's somewhat like asking how the internal combustion engine will benefit horses. The question assumes the wrong kind of change.**

> Here is a more useful attitude: Programming has to work like this. Programmers must be able to read the vocabulary, follow the flow, and see the state. Programmers have to create by reacting and create by abstracting. Assume that these are requirements. Given these requirements, how do we redesign programming?

> Another example. Most programs today manipulate abstract data structures and opaque objects, not pictures. How can we visualize the state of these programs?

> Traditional visual environments visualize the code. They visualize static structure. But that's not what we need to understand. We need to understand what the code is doing.
> > Visualize data, not code. Dynamic behavior, not static structure.
>
> > Maybe we don't need a silver bullet. We just need to take off our blindfolds to see where we're firing.

## Relevent Resources

- <https://techbeacon.com/app-dev-testing/how-learning-smalltalk-can-make-you-better-developer>
- <https://lively-kernel.org/>
- <https://amber-lang.net/>
