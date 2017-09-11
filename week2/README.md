# Week 2

# Review and Discussion of Week 1
From Silicon to Singularity

Does code belong with design?

Review of variables

[iPhone text message, emoji replacement example]

# Data Types

From the wikipedia definition states: a data type or simply type is a classification of data which tells the compiler or interpreter how the programmer intends to use the data.

[Connecting the dots, let's show where this lives in the stack from week 1]

You choose a data type for your variables according to what you want to do with them. Which operations you want to perform.


For this class we will focus some [primitive data types](https://en.wikipedia.org/wiki/List_of_data_structures#Data_types), these are types that are built in to the programming language. They can change from language to language, but the following are fairly standard across the board. 

And we will learn about some composite types, like arrays.


## Characters and Strings
A character is a single character, and string is a sequence of characters.

JavaScript example

	var myString = "Hello World"
	
Python example

	myString = "Hello World"
	
C example

	char myCharacter = 'A'; // this is just a single character
	char *myString = "Hello world"; //string literal, cannot be changed
	char myString[] = "Hello world"; //newly allocated memory

Last week's questions about single quote vs double quotes applies here to the C example, but the Python and JavaScript examples are interchangeable so long as they match.

### Delimiters

A common delimiter is a comma (,) or pipe (|). 

> A delimiter is a sequence of one or more characters used to specify the boundary between separate, independent regions in plain text or other data streams.[1] An example of a delimiter is the comma character, which acts as a field delimiter in a sequence of comma-separated values. Another example of a delimiter is the time gap used to separate letters and words in the transmission of Morse code.

[Wikipedia Definition](https://en.wikipedia.org/wiki/Delimiter)

Understanding and using delimiters in strings will be important once we get to conversion a little later in class.

### String Concatenation
Joining character strings end to end.

JavaScript example

	var myString = "Hello" + " World"
	
Python example

	myString = "".join(["Hello ", "World"])
	
C example. There is no string concatentation operator in C. Luckily, Arduino provides a nice [String](https://www.arduino.cc/en/Reference/StringObject) class with a concat method for you.

[need arduino example]


## Numbers

The two main types of numbers you'll decide between in most cases are *integers* or *floating point decimals*. Floats are used when more preceision is required.

Some things, like pi, cannot be expressed as an integer.

In Javascript, though things are rapidly changing, there is one type of [number](https://en.wikipedia.org/wiki/IEEE_754-1985#Double-precision_64_bit). Later in class during we will discuss builtin function `parseInt` and `parseFloat`.

### Integers
	-1, 0, 1, 2
    
JavaScript example

	var myInt = 1
	
Python example

	myInt = 1
	
C example

	int myInt = 1

### Floats
    -0.1, 0.0, 0.1, 0.2, 3.14

JavaScript example

	var myFloat = 3.14
	
Python example

	myFloat = 3.14
	
C example

	float myFloat = 3.14

### Further Number Types	
	    
#### NaN
Not a Number, If, for example, you attempt to divide by zero.

#### Binary and Hexadecimal
Binary representations of number use only ones and zeros. Hexadecimal can represent 8 binary characters with 2 consecutive hexadecimal digits and therefore save space.

[The Martian](http://www.businessinsider.com/the-martian-hexidecimal-language-2015-9)
[The Martian hexidecimal reference getting nerdy](https://scifi.stackexchange.com/questions/107675/why-does-mark-use-hexadecimal-to-communicate)


#### A side note about Bases

> In mathematical numeral systems, the radix or base is the number of unique digits, including zero, used to represent numbers in a positional numeral system. For example, for the decimal system (the most common system in use today) the radix is ten, because it uses the ten digits from 0 through 9.

Wikipedia definition of [Radix or base](https://en.wikipedia.org/wiki/Radix)

[Number bases introduction](http://www.purplemath.com/modules/numbbase.htm)

Binary = base 2

Decimal = base 10

Hexadecimal = base 16


    
## Booleans
A var of this type can only have 1 of 2 possible values. True or False, yes or no, on or off.
JavaScript example

	var myBool = true
	
Python example

	myBool = True
	
C example

	boolean myBool = true


## Arrays
[why can't I hold all these vars]

List of items, all of the same data type.


[Code Academy's excellent explanation](https://www.codecademy.com/courses/web-beginner-en-8a35h/0/1)

## Objects

Objects are collections of properties

# Further considerations

## Conversion from one Data Type to Another
Converting one data type to another

String -> Number

Number -> String

String -> Bool

Number -> Bool


## Strict Typing

Some languages have this, some do not.

# Madlib code example

Fun times! we will use all our new knowledge to build a mad lib 

steps to initializing a variable

1. datatype (var, int, etc... )(some languages like python you don't have to do this)
2. variable name
3. assignment operator (=, and a note on ==)
4. the value

## Readability
- easier to get help and work with others
- var myName = "firstname lastname"
- naming conventions, camelCase, snake-case
- can't start with a number

## Comments

- Comment to help others understand what your code does.

```
//, #, /** **/ ,<!-- --> 
```

# Resources

dataviz

[http://www.datavizcatalogue.com/](http://www.datavizcatalogue.com/)

javascript reference, via w3schools.com

[https://www.w3schools.com/jsref/default.asp](https://www.w3schools.com/jsref/default.asp)

javascript string documentation

[https://www.w3schools.com/jsref/jsref_obj_string.asp](https://www.w3schools.com/jsref/default.asp)

javascript number documentation

[https://www.w3schools.com/jsref/jsref_obj_number.asp](https://www.w3schools.com/jsref/jsref_obj_number.asp)

papers

[http://icee2007.dei.uc.pt/proceedings/papers/432.pdf](http://icee2007.dei.uc.pt/proceedings/papers/432.pdf)

p5 data-variables

[https://p5js.org/examples/data-variables.html](https://p5js.org/examples/data-variables.html)

ASCII chart
[ascii chart](https://upload.wikimedia.org/wikipedia/commons/d/dd/ASCII-Table.svg)