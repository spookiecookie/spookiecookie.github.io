---
published: true
title: Comparator and Comparable
layout: post
tags: [java, comparator, comparable, collections]
categories: [java]
---
Are the two things that I was not knowing well. It happened that I messed them together. They are different. 

The Comparator is defined as 

```java
    public interface Comparator<T> 
    {
        int compare(T o1, T o2);
        boolean equals(Object obj);
    }
```

and is used to compare two objects. The comparator may use different ordering strategy than one defined by natural ordering of objects compared.

The Comparable is defined as

```java
    public interface Comparable<T>
    {
        int compareTo(T o);
    }
```

and is used to impose a natural ordering on objects of the class that implements this Comparable.