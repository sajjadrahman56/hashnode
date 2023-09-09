---
title: "String Formatting in Python"
datePublished: Sat Sep 09 2023 12:54:53 GMT+0000 (Coordinated Universal Time)
cuid: clmc13h6f000108mmb99xa1ah
slug: string-formatting-in-python
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1694263955588/8723575b-0e66-4488-9e36-97497113f2b8.png
tags: programming-blogs, python, python3, mlops, sajjadrahman

---

String formatting is a fundamental aspect of Python programming that helps you create well-structured and dynamic strings. It allows you to embed variables and values into predefined placeholders within a string. In this blog, we will explore two key methods for string formatting in Python: the `.format()` method and `f-strings.`

## Using the `.format()` Method

The `.format()` method is a traditional way of formatting strings in Python. It involves using placeholders within a string and supplying values to replace these placeholders. Let's delve into some examples to grasp this concept.

### Basic Usage of `.format()`

```python
print('This is a string {} through the format method with the help of {}'.format('INSERTED', 'CURLY_BRACKETS'))
```

In this example, we have two placeholders (`{}`) in the string, and the `.format()` method takes two arguments, which are inserted into these placeholders in the order they appear.

```python
print('The {2} {1} {0}'.format('fox', 'brown', 'quick'))
```

Here, we explicitly specify the positions of the values to insert. It's important to note that Python uses zero-based indexing, so the order of insertion is 'quick', 'brown', 'fox'.

### Named Parameters

You can also use named parameters to enhance readability:

```python
print('The {q} {b} {f}'.format(f='fox', b='brown', q='quick'))
```

This approach allows you to assign values to placeholders by name, making your code more self-explanatory.

## Formatting Floating-Point Numbers

String formatting isn't limited to inserting text; it's equally valuable when dealing with numbers, especially floating-point values. You can control the width and precision of floating-point numbers using the following syntax: `{value:width.precisionf}`.

```python
result = 65 / 989
print('The result is {}'.format(result))
print('The result is {r}'.format(r=result))
print('The result is {:2.4f}'.format(result))
```

In the above example, `:2.4f` specifies that we want the result to be displayed with a width of 2 characters and a precision of 4 decimal places. You can adjust these values to suit your requirements.

## Embracing F-Strings

F-strings, introduced in Python 3.6 and later versions, offer a more concise and intuitive way to format strings:

```python
name = 'John Doe'
print(f'Hello, I am from England, and my name is {name}')
```

With `f-strings`, you simply prefix your string with an 'f' and use curly braces `{}` to directly embed variables or expressions within the string. This approach enhances code readability, particularly when working with variables.

In summary, string formatting in Python empowers you to create dynamic and well-structured strings. While the `.format()` method remains versatile and suitable for older Python versions, `f-strings` provide a cleaner and more readable option for modern Python development.

Choose the method that aligns with your project's requirements and coding style. Happy coding! Stay tuned

> Welcome to my digital corner! 🌟 Connect with me to explore insightful discussions, coding adventures, and more. Find me on:
> 
> *🐦 Twitter:* @[@sajjadrahman56](@sajjadrahman56) *🐦*
> 
> *🐙 GitHub:* [*sajjadrahman56*](https://github.com/sajjadrahman56) *🐙*
> 
> *🔗 LinkedIn:* [*sajjadrahman56*](https://www.linkedin.com/in/sajjadrahman56/)
> 
> Let's learn, collaborate, and grow together! 🚀