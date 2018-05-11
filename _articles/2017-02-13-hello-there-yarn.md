---
layout: post
current: post
cover: https://cdn-images-1.medium.com/max/800/1*vEVNlNoSTwWnO5Y2LSqdCQ.png
navigation: True
title: Hello there Yarn!
date: 2017-02-13 10:23:00
tags: programming
class: post-template
subclass: 'post'
author: thomas
---

Hello there Yarn — Goodbye NPM!
Tired of having to download the same NPM packages again and again? Then you should really check out Yarn!

Photo from https://yarnpkg.com website
Similar to NPM, Yarn is a package manager for your code, but differs on key aspects:

Firstly, when NPM or Yarn is installing packages, they both run a series of tasks, like checking for dependencies etc. With NPM these tasks are executed per package (sequentially, one at a time) while Yarn executes tasks in parallel. This makes Yarn immensely faster than NPM — in particular if you have a project with a lot of package dependencies.

Secondly Yarn is very efficient at caching already installed packages. If you already installed i.e. Bootstrap, AngularJS and ExpressJS with Yarn in another project, they will be cached so that you don’t have to download it again — saving you time and bandwidth.

An added bonus is that you can install those packages again even offline while working in the train.
