---
published: true
title: Abstract class' constructor
layout: post
tags: [abstract, class, constructor, java]
categories: [java, constructor]
---
Abstract class can have explicit constructor.

```java
abstract public class DefaultClass 
{
    int member;

    public DefaultClass(int member)
    {
        this.member = member;
    }
}


public class DerivedClass
    extends DefaultClass
{
    public DefaultClass(int i)
    {
        super(i); //some value
    }
}
```