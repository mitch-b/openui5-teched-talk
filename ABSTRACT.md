# XML Binding and Rapid Prototyping
> OpenUI5 SAP TechEd 2015 Proposal


## Abstract

TODO

## Outline

OpenUI5 makes it possible for developers (and enterprises) to rapidly build an interactive prototype which can help drive requirements gathering, and deliver solutions faster.

A key aspect to this rapid prototyping is XML views with their expression and model binding power.

Several points to touch on:

1. Why the focus on XML views instead of JavaScript?
    * Still see so many JavaScript examples online, may be that some developers are unaware that XML views exist, or how to properly use aggregations or binding in them.
    * SAP is using XML views (according to DJ Adams) for Fiori applications
    * Keep view logic in the view, while business logic remains in the controller
    * Declarative, easy to read

1. Walk through new features of XML binding and expressions coming in 1.30 release
    * [New template schema](https://openui5beta.hana.ondemand.com/#docs/guide/5ee619fc1370463ea674ee04b65ed83b.html)
    * [Expression bindings](https://openui5beta.hana.ondemand.com/#docs/guide/daf6852a04b44d118963968a1239d2c0.html)
    * Viewing debugger output from XML expression parser

1. What's so great about XML views?
    * Pass in models to multiple re-usable fragments in the same view
        * `<template:with />`
        * Demo
    * Security binding on a User model
        * Enabled/Visible
        * Demo
    * Simulating multiple user experiences with unique usage of *one-time* binding syntax
        * Demo

1. Testing
    * Mock models can be provided to views

1. Prototyping
    * Using hard-coded JSON models allow rapid iteration of UI without worrying about simultaneously maintaining your back-end service.

1. Using JSBin to ask for help
    * When describing an issue or asking another developer for help, if you can explain your problem **simply** in a JSBin (or similar service), you can either isolate the problem and resolve it yourself, or at least remove extraneous code and duplicate the issue outside of the confines of your application.
    * How to use jsbin (relate to [DJ Adams’ minimum-viable-code example](http://pipetree.com/qmacro/blog/2015/07/mvc-model-view-controller-minimum-viable-code/), and create ones with sample models in them)
    * See [these](#) examples of JSBins you can use!
        * TODO: build SPA collection that can be pasted into JSBin to demonstrate most problems
