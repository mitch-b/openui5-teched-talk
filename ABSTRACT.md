# XML Binding and Rapid Prototyping
> OpenUI5 SAP TechEd 2015 Proposal

## Abstract

OpenUI5 makes it possible for developers (and enterprises) to rapidly build an interactive prototype which can help drive requirements gathering, and deliver solutions faster.

A key aspect to this rapid prototyping is XML views with their expression and model binding power. Today, developers are still seeing many examples of JavaScript views when it comes to prototyping and searching UI5 solutions online. It may be that developers are unaware XML views exist, or how to do things like aggregations and complex binding information in this paradigm. Understanding how to translate the [JSDoc](https://openui5.hana.ondemand.com/#docs/api/symbols/sap.ui.html)s provided into usage in XML is critical.

With SAP's direction to move forward with XML views as the primary view declaration language, UI5 developers should follow suit. One of the primary advantages of this format is to **keep view-logic in the view, and business logic in the controller**. When writing your views in JavaScript, it might be tempting to add your event handlers inline, making your code harder and harder to read as you build. With XML views, the result is a clear and concise structure of what makes up your view, straight from the definition.

In the upcoming 1.30 release, UI5 will begin to provide additional functionality that makes managing your views easier with more power. With the [templating schema](https://openui5beta.hana.ondemand.com/#docs/guide/5ee619fc1370463ea674ee04b65ed83b.html), you can add conditional logic, and manage binding context for controls in an easier (more readable) way. [Expression binding syntax](https://openui5beta.hana.ondemand.com/#docs/guide/daf6852a04b44d118963968a1239d2c0.html) also has been extended to include additional objects and functionality. This will also be covered. Along with advanced expression binding, you may find your expression has failed. Demonstrating how the debugger works with XML binding will be important.

With the underlying basics covered, getting developers excited about working with UI5 is just as important. Running an interactive demo on the template schema, advanced XML expression bindings, and mock models to drive home what was previously covered will help increase this desire.

Finally, being able to properly use [JSBin](http://jsbin.com) when posting on GitHub to report an issue, or on StackOverflow to request help is vital in getting help *fast*. Covering multiple JSBin examples and going over DJ Adams' ["Minimum-Viable-Code" example](http://pipetree.com/qmacro/blog/2015/07/mvc-model-view-controller-minimum-viable-code/) will accomplish this.

## Outline

1. Why the focus on XML views instead of JavaScript?
    * SAP is using XML views (according to DJ Adams) for Fiori applications
    * Keep view logic in the view, while business logic remains in the controller
    * Declarative, easy to read

1. Walk through new features of XML binding and expressions coming in 1.30 release
    * [New template schema](https://openui5beta.hana.ondemand.com/#docs/guide/5ee619fc1370463ea674ee04b65ed83b.html)
        * Compare against wrapping a fragment in a `Panel` to achieve the same result
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
