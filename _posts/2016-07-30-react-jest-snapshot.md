---
title: React Tree Snapshot Testing
layout: post
---

I am really happy using [enzyme](http://airbnb.io/enzyme) for testing my React components. But, a couple of days ago [Facebook announced](https://facebook.github.io/jest/blog/2016/07/27/jest-14.html) a new feature on Jest: *Snapshot Testing*.

Snapshot testing is an alternate model to the typical way you would work when using Enzyme and working with the DOM. Instead, when using snapshot testing, you run Jest to create snapshots of your components and store them as text files. Every time you run Jest after that, the snapshots get compared and if they don't match the test fails. You get the option to accept the change or fix your components.

You can take multiple snapshots, for example: 
- take snapshot
- simulate a click
- take another snapshot

This is the outpur after a succesful run:

![Success]({{ site.url }}/assets/jest-snapshot-success.png)

![Fail]({{ site.url }}/assets/jest-snapshot-fail.png)

This is a great alternative when working with visual components, as it allows you to get up and running immediately with easy-to-write tests.


I've created a demo project, take a look at it here: [here](https://github.com/nicolasiugo/try-jest-snapshot)