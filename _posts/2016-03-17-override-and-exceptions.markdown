---
published: true
title: Override and exceptions
layout: post
tags: [override, exception, java, method]
categories: [java, override]
---
Methods from base class can be overriden. Methods that throw exceptions however should be overriden with care.

Repeat like a mantra: in overriding method the exception in `throws` can be

* the same exception as the exception in overriden method, 
* the subclass of the exception in overriden method,
* the RunTimeException and it's subclasses,
* no exception at all (then no `throws` used in declaration).