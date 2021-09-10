# Email regex-tutorial

Introductory paragraph (replace this with your text)
if you have signed up for a free-trial for Disney + or many other websites you have probably signed up with your email so they can send you annoying emails and will conviniently stop when the trial expires and they charge you $15. But how do those company check to see if its an actual email and not just random gibberish (ex: jtuoshhaoeoj). Companies will do this by using a regex.

## Summary

I will be showing a tutorial on email regex's and an email regex will look typically like this: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

I will going over what each of these code snippets mean over the course of this readme.


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components
first off let's look at the brackets and the characters within. [a-z0-9_\.-],[\da-z\.-](yes there is a difference), [a-z\.]{2,6}.

the [a-z0-9_/.-] tells the computer to accept any characters within these parameters. Aforementioned characters include the entire alphabet numbers 0 to 9 and underscores, hyphens and, periods. 

[\da-z\.-] does mostly what the previous bracket session does but specifies that this must be a domain gmail, yahoo, hotmail(for those who were born before 2004), amazon, comcast, etc... and must be ended with a period.

[a-z\.]{2,6} is where the .com, .org, .net and all those go. the unique aspect is that the {} adds a character limit wehre the first argument goes for the minimum and the second argument sets a character limit ceiling.


### Anchors
to move next we have to look at the beginning and end. AKA \^ and $/ which are known as anchors. Essentially ^ starts a string and $ ends the string, there are other anchor arguments but I dont have to talk about those.


### Quantifiers

quantifiers match character lengths come in 4 exciting shapes and sizes +,*,? and,{}(i've briefely talked about this). 
'+' means one or more. This is signified with the (+@) which makes the user put in an @ sign after entering their characters.

'*' means 0 or more and isnt showed in my particular regex so I'm not talking about it.

? activates a boolean response of being either 0 or 1. Or if you're in Star Trek blink 0 for yes, blink 1 for no. 

{} is the one I talked about earlier, it sets a minimum and maximum lengths


### Grouping Constructs

grouping constructs are the parenthesis that cover the brackets and plus sign (). setting the three sections into there own seperate spaces 1: person@ 2:gmail. 3:com. 

### Bracket Expressions

this is the \d in the second session and puts specific parameters on character classes

### Character Classes
 [] set a limit of what specific characters you can put into that specific area.


### The OR Operator
the OR operator is not used in my regex but I'll still talk about it. the OR operator is signified by | and if it looks vaguely familiar its because we used it in javascript as a way to accept one set of script or another.


### Flags

/ are different from \ and in a nutshell tells javascript and it better buckle its seatbelt because it is heading into a regular expression

### Character Escapes

\ is a character escape and tells the regex to get out of any special characters it might run into 

## Author

Hi! My name is Rob Simanton, I enjoy coding, excel, and, not writing serious papers. I am currently in college pursuing a finance degree while pursuing this web development course. I am fascinated by the absolute creativity that comes with Web Development and the real-world impact I could have with doing finance.

https://github.com/RSimer