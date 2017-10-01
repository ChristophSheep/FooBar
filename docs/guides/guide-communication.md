## Communication

### Introduction

see https://en.wikipedia.org/wiki/Communication

Today we communicate through our source code with other developers.

We do not write big documentation. 
We do not even write a short method or class descriptions.

### Problem

In any language we communicate through words and signs.
We learn the meaning of that and we communicate our
meaning through words and signs.

#### Poor coding style like poor handwriting style

Like there is standard way of writing letters everyone can read. 
There should also standard way to write code.

Some have a coding style that looks like poor handwriting.
Also the project structure looks like poor handwriting.
Only the one who wrote can read and know where to find the classes. 

So it is more a cryptographic style of coding. Who reads it
need a lot of headache pills.

#### Poor coding style like a poor dialect/slang

Like in every human language some coding style looks
like a special dialect and if you read the code you
can not easily understand the code.

If someone writes a technical documentation for others
but nobody could read it, because of his bad handwriting
what is the point of that. It make no sense.

#### Communicate through Project Structure

In my opinion if two company create an application, 
the project structure should be look very similar.
So if you swap developers, they should find easily
the way in the project structure. 
If they seek the business entity object they should
find it on a place where they expect it should be.

There should some kind of standardization how a project
structure should look like.

#### Comparison with a House

Basically every house have the similar structures.
It has a basement and first floor, some other more
floors and a roof.

You would not expect the roof at the place of the
basement. Or you would not expect the basement at the
top of the house.

Its sound perhaps silly, but I have seen projects where
you can not find the classes where you expect them.

So you always have to seek and get a headache over day.
And your brain get very confused the more you work
with that kind of project because there seems no pattern
that you can learn. It only a mess.

### Solution

In my opinion we should have similar project folder.
Each project should have a "ViewLayer" project and
"BusinessLayer" Project and "DataLayer" project.

Solution FooBar

 -> Project "Aspects"
  | -> Link View        (Top Layer)
  | -> Link ViewModel
  | -> Link Presenter
  | -> Link Business
  | -> Link Storage     (Bottom Layer)
 
 -> Project "View"
  | -> View.cs
  | -> ViewModel.cs
  | -> Presenter.cs
 
 -> Project "Business"
  | -> Class FooObj
  | -> Class BarObj
 
 -> Project "Storage"
  | -> Class DbStorage.cs

#### Rules

Rules how to create a proper project structure.
Rules how to right proper code.


