---
layout: essay
type: essay
title: JavaScript Doesn't have a Type
# All dates must be YYYY-MM-DD format!
date: 2020-01-22
labels:
  - JavaScript
  - Java
  - Coding
---


 <div style="text-align: right"> <img src="../images/javascript-doest-have-a-type-comic.png">

You can just declare a function. Yes, as a keyword. Just make a standalone function and call it. Don’t worry about what it’s going to return we can make it up as we go along, more in just a second.

## The Good

Having a background in primarily Java and C the idea of being able to haphazardly throw items into an array like potatoes into a sack was a bit concerning. Then I thought why does Java need to know what’s being stored in an array? I myself couldn’t come up with a good answer for that. While it does make it neater from the perspective of you aren’t getting a string out of your integer array it makes it more cumbersome when you need to store a few of integers strings and chars for example. Then you are trying to decide if you should make an array for each type or just have a bunch of variables. No matter which you pick the argument could be made for the other.

## The Better
Objects are also easier to use in JavaScript. With arrays being easier to use this by extension objects easier, because objects are just a collection of properties under a single name kind of like an array. Accessing the information out of an object is similar you can use the dot notation to access a property of the object, or bracket notation. JavaScript is flexible though, if you forgot that your person object should have a field for say age you can add it by executing the code below:
```
let person = {firstname: "Joe", lastname: "Smith"};
console.log(person.firstname); //prints Firstname
person.age = "21"; //add age property after
console.log(person.age);//18
```
This is a breath of fresh air coming from Java and makes fixing things as you go much easier.

## Get Your Time Back

While my JavaScript knowledge is still quite fresh by using a different learning approach it has made learning it and retaining it easier. The new method I was using was timed problem solving. In the hustle and bustle life of the 21st century doing timed exercises may not sound like a huge deal. However, it can greatly improve competency in a short amount of time. Usually coding assignments allow for flexibility. You can do it all at once or you build it over the course of the deadline. Adding the time factor forces you to think and type quickly while attempting to arrive at a solution. It also gives a definitive measuring stick in how well you did when compared to your peers or to your previous attempts. As my life gets more and more hectic completing smaller tasks quickly gives me more time overall in my day.
