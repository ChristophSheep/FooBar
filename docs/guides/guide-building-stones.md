# `Building Stones`

## Introduction

Building stone are very general made core classes.
Which this classes you can build any kind of different
application.

With claybricks you can build any kind of different
houses. You can build small one family house or a big
church building or a university or concert hall.

## Solution

Use a good framework, but also build on that your own
application independet classes for every layer (View, Model, Storage, ...). Try to build them as general as possible without think
for what you will need it later.

I worked for a company where we had a core class name ObjectWithAttributes and class ObjectWithAttributesList.
also with had Attribute class for every kind of different
Attributes. 

We these class he could build a very general usable UI and
store them very general in the DB.

We could build or own property editor for this core class
and or own dataGrid View like control to view list of
objects with attributes.

If you at a new entity that was derived from this core class
everything worked on the UI without any change to made.
This is a good sign of a healthy application. It just still
works. You only have to implement a new type by implementing
the interface and its seamless integrate into the system. It
also could be done at runtime like plugins.

This core classes we used for a graphic viewer as well for a
document management system. So this classes were very general made.

So you had the feeling that you have a higher set of building stones
instead of simple classes. We simple class you need your extra
forms elements to edit them. You need you own tables in the Db to
store them. Extra query to load and store them back. So application
in growing and growing with every new content type. 

Which is more like weed and a healthy organismus. (see Weed Seed Guide too)

### Example PseudoCode ###

Following classes or higher then normal classes.
A class of a language is a building stone and
with this small stones you can build more general
higher level "class-like" building stones.

A property in a normal class is self a class.
instead of using a string for a Name property. 
You use a NameAttribute class.

Instead of

```C++
class Person : AObject
{
    int     Id;
    string  Name;
    int     Age;
}
```
You use something like that
```C++
class Attribute
{
    string  Type;
    object  Value;
}

class AttributeName : Attribute
{
    string  GetName(Culture);
    string  FriendlyName(Culture);
}

class AttributeId : Attribute
{
    int Id;
}

class NumericAttribute : Attribute
{
    decimal Value;
}

class ObjectWithAttributes
{
    int         GetAttributesCount();
    Attribute   GetAttribute(int index);
    Attribute   GetAttributeByName();
}

class Person : ObjectWithAttributes
{
    IdAttribute        Id;
    NameAttribute      Name;
    NumericAttribute   Age;

    Person()
    {

    }

    int GetAttributesCount()
    {
        return 3;
    }

    Attribute GetAttribute(int index)
    {
        if Index == 0 return Id;
        if Index == 1 return Name;
        if Index == 2 return Age;

        throw IndexOutOfRange;
    }
}

```



## Problem

If you do not have building stone that your application
will grow and grow with classes and it will get hard to
maintain. Because your code bases will be to big.
Any changes and every application who lives long hasto change
over the years. Life is dynamic. Needs of customer change.

