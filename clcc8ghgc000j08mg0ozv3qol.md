---
title: "My Dev Retro 2022"
datePublished: Sat Dec 31 2022 17:43:54 GMT+0000 (Coordinated Universal Time)
cuid: clcc8ghgc000j08mg0ozv3qol
slug: my-dev-retro-2022
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1672506857067/3831b77a-3ff6-4cd5-bc03-382a2e6a3c8f.jpeg
tags: devretro2022

---

Flutter development is the first development in my life so far. As a newbie, I have been facing a number of errors in science since the start. I heard one of my mentors say that the more errors you make, the more you learn.

## What is Flutter Development?

Flutter apps are written in the Dart language and use many of the language's more advanced features. 

While writing and debugging an application, Flutter runs in the Dart virtual machine, which features a just-in-time execution engine. This allows for fast compilation times as well as "hot reload", with which modifications to source files can be injected into a running application. Flutter extends this further with support for stateful hot reload. In most cases, changes to source code are reflected immediately in the running app without requiring a restart or any loss of state. \[ [source](https://en.wikipedia.org/wiki/Flutter_(software)#:~:text=Flutter%20is%20an%20open%2Dsource,web%20from%20a%20single%20codebase.&text=First%20described%20in%202015%2C%20Flutter%20was%20released%20in%20May%202017.) \]

## My First API Call?

The thing I am going to share with you guys is the Networks call ( get, post ) in Flutter. This is very important to know how to connect Networks in your project whether the development is in any language. 

I watched many videos and then I tried to apply for my project. Whenever I am going to apply, I get stuck.

My first API call is weather API from open API. We all know this is a famous weather API. Oh, I forgot to mention that my project name is weather API. A very simple project but as a beginner, I felt this is a very challenging one. 

At first, I did UI design and then I wanted to connect to the API. I got a number of errors but I am so poor that I could not fix the errors that were given to me. After two days I was able to mark my URI parsing method as wrong.

## Flutter HTTP Package

I used the HTTP package \[ [https://pub.dev/packages/http](https://pub.dev/packages/http) \] 

This is the demo code 

`import 'package:http/http.dart' as http;`

`var url = Uri.https('`[`example.com`](http://example.com)`', 'whatsit/create');`

`var response = await` [`http.post`](http://http.post)`(url, body: {'name': 'doodle', 'color': 'blue'});`

`print('Response status: ${response.statusCode}');`

`print('Response body: ${response.body}');`

`print(await` [`http.read`](http://http.read)`(Uri.https('`[`example.com`](http://example.com)`', 'foobar.txt')));`

Before I explain my problem, I will describe more about get put and post.

### GET

Get the method used to collect something from API.

### PUT and POST

These two are few /similarities but they are quite different. In the put method, it gives the same result if we call more than once, on the other hand in the POST it gives a different result for each call. 

**Put use for update query where POST use for CREATE query.**

The below picture it will help a little more to understands

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672506695904/ebbc8db1-e4e9-4689-bde8-b6838e0dcaa7.png align="center")

Back to the code that I made mistakes in, I used the Uri method instead of `Uri.https` . The problem occurs because I am less careful because I pass the wrong parameters. As a result, the code is not working. After that, I am available to fix this problem but I was interrupted by another new problem which was `lat and lan` passed. Lat and Lan are nothing but the acronym of Latitude and Longitude respectively. That gives the position or location of any place on Earth’s surface that can be determined and described.

Finally, I am able to pass those parameters, and the code run perfectly. I used [openweather](https://openweathermap.org/) map as API.

## My Learning

Development is really fun when the code is work perfectly. I learn how to call API calls. my output is

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1672508135626/a62ee61a-a32c-4326-b535-bc713dab3aa1.png align="center")

# Pardon 🙏

This is for the very first blog on this site, also my entire journey. I know my writing style is not good, but I will try my best. Please give me suggestions.

Thank You!

*you can connect with me*

@[Sajjad Rahman](@sajjadrahman)

%[https://github.com/sajjad-njr]