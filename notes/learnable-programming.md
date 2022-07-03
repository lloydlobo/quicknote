---
id: 4nbo4cbcvioulri6o0q1esm
title: Learnable Programming
desc: ''
updated: 1656824111470
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
  - [See the state](#see-the-state)
  - [Create by reacting](#create-by-reacting)
  - [Create by abstracting](#create-by-abstracting)
  - [Language](#language)
  - [Great works](#great-works)

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

### See the state

### Create by reacting

### Create by abstracting

### Language

> A programming system has two parts. The environment is installed on the computer,
> and the language is installed in the programmer's head.

### Great works

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
