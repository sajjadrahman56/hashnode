---
title: "String  in Python - 2"
datePublished: Wed Aug 23 2023 13:21:17 GMT+0000 (Coordinated Universal Time)
cuid: cllnrjy3j001h0alf8e6w1jxk
slug: string-in-python-2
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1692796807066/74a782d3-e61a-4004-b329-59622125b606.png
tags: programming-blogs, python, machine-learning, python-beginner, sajjadrahman

---

### Immutability of Strings

Strings are a fundamental data type in Python, serving as a sequence of characters. However, one key property of strings is their **immutability**. This means that once a string is created, its individual characters cannot be changed. Let's delve into this concept with an example:

```python
name = "abir"
name[0] = 'p'  # This will raise a TypeError
```

Running the above code snippet will result in an error: "TypeError: 'str' object does not support item assignment." This error demonstrates the immutability of strings, preventing direct modification of characters.

### Replacing Characters in a String

While you can't modify characters in an existing string, you can create a new string with desired alterations. For instance, let's assume we have the string 'abir', and we want to replace the first character <mark>'a' with 'k</mark>'. Here's how to accomplish it:

```python
name = "abir"
last_letters = name[1:]
new_name = 'k' + last_letters
print(new_name)  # Output: "kbir"
```

In this example, string slicing is used to extract characters without the first one. By concatenating the desired character ('k') with the sliced portion, the new string 'kbir' is formed.

### String Multiplication

Python permits us to multiply strings to repeat them a specified number of times. For instance:

```python
first_name = 'Jon'
multiplied_name = first_name * 10
print(multiplied_name)  # Output: "JonJonJonJonJonJonJonJonJonJon"
```

Here, the string 'Jon' is multiplied by 10, leading to the repetition of the string 10 times.

### Changing Case (Upper and Lower )

We can change the letters smaller to capital by use of `upper()`, and vice versa.

```python
jon = " hello bangladesh mlops club"
upper_case_jon = jon.upper() 
print(upper_case_jon) # Output: " HELLO BANGLADESH MLOPS CLUB"
```

### Splitting Strings

The `split()` method divides the string into a list of words, like`['hello', 'bangladesh', 'mlops', 'club']`.

```python
jon = " hello bangladesh mlops club"
split_jon = jon.split()
print(split_jon)  # Output: ['hello', 'bangladesh', 'mlops', 'club']
```

The `split()` parameter is null which means when it finds the space then the split() words. We can pass a parameter inside the method like `split('a')` and then look at the example

```python
jon = " hello bangladesh mlops club"
split_jon = jon.split('a')
print(split_jon)  # Output: [' hello b', 'ngl', 'desh mlops club']
```

### More Methods

### *Remove leading and trailing whitespace*

```python
sentence = " Python Programming is Amazing       "
cleaned_sentence = sentence.strip() 
print(cleaned_sentence) # Output: "Python Programming is Amazing"
```

### *Count the occurrences of a substring*

```python
sentence = "Python Programming is Amazing"
count_amazing = sentence.count("Amazing") 
print(count_amazing) # Output: 1
```

### *Check if the string starts with a certain substring*

```python
sentence = "Python Programming is Amazing"
starts_with_python = sentence.startswith("Python") 
print(starts_with_python) # Output: True
```

### *Replace a substring with another substring*

```python
sentence = "Python Programming is Amazing"
new_sentence = sentence.replace("Amazing", "Incredible") 
print(new_sentence) # Output: " Python Programming is Incredible "
```

## Conclusion

In this tutorial, we delved into the immutability of strings and explored various string methods that enable us to manipulate and process textual data effectively. By understanding the principles of string immutability and harnessing the power of string methods, you can create more dynamic and flexible programs for handling string-related tasks.

For more learn about string methods please go here [python documentation](https://docs.python.org/3/library/string.html)

<div data-node-type="callout">
<div data-node-type="callout-emoji">💡</div>
<div data-node-type="callout-text">Comment your thoughts</div>
</div>

🐦 Twitter: [@sajjadrahman56](https://twitter.com/sajjadrahman56) 🐦

🐙 GitHub: [sajjadrahman56](https://github.com/sajjadrahman56) 🐙

🔗 LinkedIn: [sajjadrahman56](https://www.linkedin.com/in/sajjadrahman56/)

@[Sajjad Rahman](@sajjadrahman56)

Stay connected and follow me on my social media accounts to keep up with my latest updates and projects! 🌟 Let's collaborate and share knowledge. 🤝 Looking forward to engaging with you in the tech community! 👩‍💻👨‍💻