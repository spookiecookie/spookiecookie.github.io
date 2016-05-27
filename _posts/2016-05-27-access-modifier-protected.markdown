---
published: true
title: Access modifier protected
layout: post
---
Access modifier protected allows to access instance member of the class from other package or instance member of the base base class by using inheritance... but not using reference variable.

```java
package bpackage;
public class Base 
{
    protected String member = "value";
}


package dpackage;
public class Derived 
    extends Base
{
    public void accessMember()
    {
        System.out.println(member);     //this works      
    }
    
    public void accessMemberByReference()
    {
        Base b = new Base();
        System.out.println(b.member); //compilation-time error  :)
    }
}
```