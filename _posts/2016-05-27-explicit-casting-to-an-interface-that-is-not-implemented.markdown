---
published: true
title: Explicit casting to an unimplemented interface
layout: post
tags: [java, explicit, casting, interface]
categories: [java, casting, interface]
---
Explicit cast of a variable to an interface this variable's class doesn't implement is allowed at compile time.

```java
public interface Blog 
{
}

public class Book //doesn't implement Blog interface
{
}

public static void main(String[] args)
{
    Book book = new Book();

    Blog blog = (Blog) book; //allowed at compilation though will fail with RuntimeException ClassNotFoundException at run-time.
}
```