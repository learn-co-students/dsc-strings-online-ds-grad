
# Introduction to Variables: Strings

## Introduction
As we already know from living in the digital age and the lessons we've already seen, programming is a powerful tool for answering questions about data. It allows us to collect, clean up and format our data and then perform calculations on that data.

Much of our digital information is in the form of text, for exmaple song lyrics and emails. To clean up and format that text with Python, we need to become familiar with our first type of data, the String.

## Objectives
You will be able to:
* Understand and use the data type, Strings
* Understand, explain and use the correct data types for various types of information (strings)

## What Are Strings?

A lot of information in the world is in the form of text. To capture this information and operate on it in Python we take this text and make it into the **String** (`str`) data type.

Below, we have the name of a cartoon character, Homer Simpson. By putting quotes (`""`) around the name, we create a string.

```python
"Homer Simpson"
```
When programmers say *string*, what they mean is text.  When programmers say *data type*, they just mean type of data.  We can think of `'Homer Simpson'` as an instance of the string data type.

Here are a few other types of data in Python that we will talk more about in later lessons:
```python
100 # Integer
10.0 # Float
True # Boolean
```

Since there are several types of data in Python we can discover the type of any piece of data by calling, or executing, the `type()` function. By calling or executing a function, we mean running the function so that it executes the code within it.

Let's look at an example below:

> **Note:** Press the shift + enter keys to run the code below. The cell that populates below is the return or output of the type function.


```python
type("Homer Simpson")
```

We need to pay attention to what type of data we are working with because they operate differently and have different values as well as functions that we are able to use on them. 

For example, to create a new string (or to *initialize* a string) we cannot simply type letters. Instead, we need to be very explicit and tell Python it is about to see some text. We do this by surrounding our text with quotes, `""`.  If we don't do that or end our quotation marks too early, Python will throw an error.

## "This is a properly formatted string!"


```python
"Th"is will throw an error!
```

> **Note:** double quotes and single quotes can be used interchangeably in Python; however, for readability it is important that we stay consistent. At first, it might seem strange how picky programmers are about details like this, but after a couple of years of coding, you too might end up in a fight like [this one](https://www.youtube.com/watch?v=SsoOG6ZeyUI)!

### Changing Data With Built In Methods

Python is picky like this for a reason. For example, once it knows we are working with a string, it gives us specific functionality for operating on strings. We call this functionality a function or a method.

Below we have a method that works with a String, but does not work with a Boolean.


```python
'Homer Simpson'.upper()
```


```python
42.upper()
```

Yep.  Bad news bears.

As we can see in the examples above, we can operate on a datatype using the following format: 

   * [INSTANCE OF A DATATYPE] [DOT] [METHOD NAME] [PARENTHESES]

Here are some more examples that follow this format:


```python
"Homer Simpson".endswith('Simpson')
```


```python
"Charles Montgomery Burns".endswith('Simpson')
```

As you can see, most of our operations on data will follow the data-dot-method name-parentheses format.

###  Discovering New Methods

You may be starting to worry about there being too many methods to keep track of. Let's ask Python for help with finding more information about what we can do with strings.

The `help()` function in Python comes built-in and is like an old school Alexa. We give our prompt or *data type* to the `help()` function and it tells us everything it knows about that data type.

Let's see what happens when we type `help(str)`.


```python
help(str)
```

So, we can see from the output it gives us a lot of information regarding the datatype including built-in methods we can use to operate on data of that particular type (i.e. Strings).

**Note:** *If you type the `help()` function in your terminal and the output is longer than the window, you can press the letter `q` to exit back to normal operation.*

Holy cow that's a lot of words. If we scroll down to the word capitalize, things begin to make more sense. For example, for capitalize, this is what it says:

```python
capitalize(...)

    S.capitalize() -> str
    Return a capitalized version of S, i.e. make the first character
    have upper case and the rest lower case.
```

Our next step is to use our formula of datatype-dot-method name-parentheses, and see what happens next.


```python
"smithers".capitalize()
```

## Tips going forward

That's really it for this lesson on strings, and it's easy to feel a little unsatisfied with just a few methods on the datatype. What's more important with programming is mechanisms of discovery and experimentation beyond just memorizing a list of features.

In this lesson, we already saw a few of them.
* Guess: We just tried something and looked to the error message for clues as to what to do next.
* help(str): We saw a nice way to learn about new methods, then we took a guess to test our understanding
* Following a pattern: We started with a simple method like calling upper, took a moment to break this down into a pattern, and then tried this pattern again to call other methods

Here is one more method of discovery:  **just ask Google**.  For example, look what happens when we ask Google about capitalization.

![](https://learn-verified.s3.amazonaws.com/data-science-assets/ask-google.png)

[A great link with a detailed answer.](https://stackoverflow.com/a/1549644)

![](https://learn-verified.s3.amazonaws.com/data-science-assets/stack-overflow.png)

Then we try this new method out ourselves, to see if this user on StackOverFlow is right (they normally are).


```python
"hello world".title()
```

And our work is done.

Feel free to look at [other common string operations here.](https://docs.python.org/2/library/string.html)

## Summary
In this lesson, we learned about our first datatype in Python: the string.  A string is just text. We indicate to Python that we are writing a string by surrounding our content with quotation marks. Once we do this, we can operate on this string by calling methods like `upper` or `endswith`. We identified a general pattern for calling methods on datatypes: 'instance of a datatype-dot-method name-parentheses'.

The second thing we learned was different mechanisms for learning about methods.  We saw the importance of guessing and experimentation, and how doing so can give us error messages, which provide clues. We also saw how to ask questions about a datatype by calling 'help' followed by the datatype name like `help(str)`.  Finally, we saw we can ask Google.  This mechanism of exploration is a skill we'll build up over time and this course will provide guidance and practice on along the way.
