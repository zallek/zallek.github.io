---
title:  "The problem of React Open Source components customization"
description: Work in progress
## date: add a date when publishing
---

For the last 6 months, we have been starting to integrate more and more [React](https://facebook.github.io/react/) components in Botify SaaS application, initially developed with Chaplin on top of Backbone.
I might create a post about it to explain how we did it, what we used, what issues we encountered and what do we still have to do. But that's not the point of this post. 

This experience allows me to use the React on a real project that is shipped in production every day. I really like how it allows to create reusable composable components, with a self-documented interface in a declarative way that make it less buggy and much more easy to maintain. I love the concept of immutability, functional programming it brings and how it suits well with the new ES6 features. I wouldn't come back 6 mounts later when we were developing jQuery pieces of code on top of Handlebars templates.

# The problem
But React becomes to be really a pain when it comes to using or developing open source components. Why? Because **when you use an open source component you need to be able to customize it**. But the way React is made make it impossible to modify the rendering like we can do with jQuery plugins or Angular directives by listening to lib's built-in events or DOM events and modifying the DOM.

Thought, being able to customize the style of a component, alter its behavior, or add some features is a real need. Maybe not right now, but later. 

# Example 1: The missing feature
Consider the following situation: you are being asked to integrate a new table displaying data in a paginated way. As you don't what to reinvent the wheel for something so common and you are a small team or maybe  even alone, you decide to use an open source component. So you spend some time studying available project and finally choose one that fits your needs and seems sufficiently maintained. You develop your thing and move on. But sometimes later, you are being asked to add buttons on hover to delete columns. And you are stuck because the component you chosen doesn't propose that and isn't enough customizable to allow it. 

So you have no choice that either trying to make the product team reconsider that idea or explain to them that it will take hours because you need to change the whole component, process data in another way that fits you new component and so on.
That's happened to me, and be sure that my boss wasn't so happy.

# Example 2: The styling problem

# What we did


# What I propose


I understand that it's not a problem for Facebook that have hundreds of developers to create their 15k + in-house components. But I would appreciate that they consider thinking about it.
