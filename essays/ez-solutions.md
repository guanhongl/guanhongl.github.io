---
layout: essay
type: essay
title: "EZ Solutions to Your Problems!"
# All dates must be YYYY-MM-DD format!
date: 2020-12-02
published: true
labels:
  - Design Patterns
---

## The Assembly Line of Programming

Imagine that you are a software engineer and you encounter a problem regarding coding structure or implementing an efficient user interface separate from the internals of your system. What if there were templates made by brilliant computer scientists that you could readily use to solve such problems? This is what design patterns are! They are formal ways and best practices for solving recurring problems in software design. I find design patterns similar to the manufacturing of cars. All cars go through the assembly line in which different parts are logically and methodically assembled to ramp up production. Much like the assembly line, design patterns are universal solutions and templates used in software design.

## Untangling Code

I recall my early days in computer science where entire programs were defined and written in a single class. Some refer to them as 'God classes': classes that do everything and are often hundreds of thousands of lines of code. Such classes are a tangled mess of code; they lack structure, cleanliness, and formality. However, design patterns offer ways to manage the complexity and structure of your code. For example, one might use the Factory design pattern to return objects of different classes without exposing its creation logic. One might also use the Model View Controller (MVC) design pattern to organize code in a way that separates the model from the ui.

## Already in Use?

You may already be unknowingly using design patterns in your code seeing as how they are best practices. I didn't recognize the design patterns I'd been using in my code until recently. Meteor inherently utilizes the Publish-Subscribe design pattern through its pub-subs. In my final project, I'm able to decide what data the server publishes and which clients subscribe to which publishers. For example, in the profiles collection, I may publish only the profile specific to the user. There is also the Singleton design pattern which makes it so there is only a single instance of a class. `Profiles` may be the single instance of the profiles collection class where the profiles collection can only be modified by methods called on `Profiles`. However, the design pattern I view as the most useful in web design is the MVC. The model contains the database, the view contains the ui, and the controller mediates between the model and the view. This enables programmers to divide their program into three separate parts. In Meteor, we use MongoDB (M), React (V), and Meteor (C). The MVC enables three different groups to work on the same program without stepping over another. Design patterns add uniformity to programs; they organize code in ways that are easy to understand and reuse.