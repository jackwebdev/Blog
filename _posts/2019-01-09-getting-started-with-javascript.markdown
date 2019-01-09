---
layout: post
title:  "JavaScript Slang - Knowing The Jargon"
date:   2019-01-09 14:28:25 GMT
categories: JavaScript
image: "/Blog/assets/images/javascript.png"
---

## What is JavaScript?
JavaScript or JS for short. It's commonly known as the programming language that runs in web browsers. Wikipedia defines it as["high-level, interpreted programming language that conforms to the ECMAScript specification."](https://en.wikipedia.org/wiki/JavaScript){:target="_blank"} 

JavaScript is also an untyped programming language. You don't need to declare the type of variable you're working with. For example in other programming languages they will want you to be explicit and tell the computer you are creating a *String*, but JavaScript will assume you typed a *String* and is implicit. For those new programmers, a *String* is a data type that allows us to store a sequence of characters. Data type referes to types of data that can be stored into variables.

### What exactly is a High-Level Language?
If you are new to programming it can be confusing as there are many different programming languages. The diagram below provided by [justcode.me](http://justcode.me) shows a diagram that is split in half representing "High-Level Languages" and "Low-Level Languages". JavaScript fits into the "High-Level" section which is not shown in the diagram. 

You might be thinking that High-Level is simply more advanced and better, but this isn't the case. It's a way to categorise. High-Level Languages are easy for us humans to understand 👽. It will contain real English words and coding is more concise. Low-Level Languages, on the other hand, are simply a language the machines understand. Low-Level languages run very quickly on the computer, but require you to direct memory management. 

- **High-Level Language**: Code that is in a human-readable format.
- **Low-Level Language**:  Code created for machines to understand.

![Programming Level Diagram. Split into Low-level and High-level](https://cdn-images-1.medium.com/max/800/1*-OVqIc67l_mzm-M6raZeCA.png)

### What is an Interpreted Language?
An Interpreted Language is where the instructions are not executed by the machine, but read and executed by some other program. JavaScript is run by a JavaScript Engine, which the engine runs the instructions. A Compiled Language is where the program is compiled into Machine Code (Binary) which the computer runs the program.

JavaScript is very Dynamic for developers to add new code while the program is running. This is because JavaScript is an interpreted Programming Language.

- **Interpreted Language**: Code executed by a separate program often called an engine, for example, JavaScript Engine.
- **Compiled Language**:  Code that needs to be packed into binary code for the computer to execute that program.

## What is ECMAScript?
This is a confusing topic! A bit like "Chicken or the egg!" 🐣

ECMAScript is the specification for creating a general purpose scripting language. [Ecma International](https://www.ecma-international.org){:target="_blank"} have the [Specification in this PDF](https://www.ecma-international.org/publications/files/ECMA-ST/Ecma-262.pdf){:target="_blank"}. ECMAScript provides the rules and guidelines that scripting languages must comply with to become a Scripting Langauge. 

**For short Ecma International provide the specification, to build a Scripting Language. JavaScript is how you use a Scripting Language. ECMAScript is the standard, while JavaScript is the most popular implementation of that standard.**

### JS, ES5, ES6 and beyond
Let's start with the crazy acronyms.

1. **JavaScript or JS** - Was named JavaScript and is not to be confused with the Java programming language. JavaScript is to Java what an Orange is to an Apple, they're not the same. JavaScript's name is the result of a marketing stunt to attract more developers during the success of Java.

2. **ES** - Put simply ES is short for ECMAScript. When you see ES followed by a number or the year it was released, it's referencing an edition of ECMAScript. 

### ECMAScript versions
- **ES1** - June 1997
- **ES2** - June 1998
- **ES3** - Dec 1999
- **ES4** - Abandoned: Due to political reasons over language complexity.
- **ES5** - Dec 2009: An amazing 10 years later!
- **ES5.1** - June 2011
- **ES6 / ES2015** - June 2015: This is where it gets confusing (Because ES2015 looks like it should be ES5 but it's not. 🤷🏻‍♂️). ES6 and ES2015 are the same things. They started adding in the year after ES. 
- **ES7 / ES2016** - June 2016
- **ES8 / ES2017** - June 2017
- **ES9 / ES2018** - June 2018

Each new update brings new features to the language.

## Little Bit Of History
Some interesting History of JavaScript. JavaScript was released on the 4th December 1995. In 1995 [Brendan Eich](https://en.wikipedia.org/wiki/Brendan_Eich){:target="_blank"} was recruited by [NetScape](https://en.wikipedia.org/wiki/Netscape){:target="_blank"} and created a prototype within 10 days during May 1995. Netscape realised the web needed to be more dynamic and needed a scripting language that had to have a syntax similar to Java's, which is why they had to build a new language and ruled out adopting other languages like Perl, Python, TCL and Scheme. We know today that JavaScript is completely different to Java. JavaScript's first code name was Mocha, later NetScapes marketing changed it to LiveScript. The Java Programming Language was growing huge so the language was renamed again to its final name, JavaScript.

To make things even more confusing you may have noticed that JavaScript started in 1995, but ECMAScript first version launched in 1997? JavaScript was submitted to Ecma International in November 1996 by Netscape for standardisation which resulted in ECMAScript. JavaScript conformed to ECMAScript specification, resulting in JavaScript being an implementation of ECMAScript.

ECMAScript is standardised from JavaScript and JavaScript conforms to ECMAScript. 😱

## Key Takeaways:
- JavaScript follows the ECMAScript specifications, JavaScript is the most popular implementation of ECMAScript specifications.
- JavaScript is a high-level, interpreted programming language.
- New versions of ECMAScript are named numerically by 1 or the release year. Starting 2015, marked with their year. E.g ES6 and ES2015 are the same versions.

### References 
- [SpeakingJS](http://speakingjs.com/es5/ch04.html#ftn.id1080022){:target="_blank"}
- [WikiPedia JavaScript](https://en.wikipedia.org/wiki/JavaScript){:target="_blank"}

