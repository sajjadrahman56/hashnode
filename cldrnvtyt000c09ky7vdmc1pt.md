---
title: "5th week of 52 weeks"
seoTitle: "how I am passing my 5th week days"
datePublished: Sun Feb 05 2023 17:31:59 GMT+0000 (Coordinated Universal Time)
cuid: cldrnvtyt000c09ky7vdmc1pt
slug: 5th-week-of-52-weeks
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1675618102101/6392f996-d0a5-4bec-b7bf-a2aa04df35a9.png
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1675618268099/7ed114ff-a4fe-4e19-873e-88bb46ae7094.png
tags: beginners, hashnode, beginner-blogger, 52weeks, sajjadrahman

---

## Jan - 30

I woke up early in the morning and watched a video on how to use reflection and deserialization My task is to serialize an object in C# without the use of the Newtonsoft.json framework.  I tried hours after hours but I couldn’t find any way. I realized how noob I am in terms of thinking. 

After a while, I noticed I have a computer Graphics class at my college with Ebrahim sir. I packed my bag and had my lunch within 30 minutes. The distance between my College and home is nearly 15 km. I felt bored with the journey as the transport system is not well alongside the traffic jams. On the bus, one boy tried to open the window but couldn't open it. He applied force as a result the glass broke and he was injured. 

When I reached the campus I talked with one of my course teachers who gave me a B grade in a course where I am confident that I should achieve an A grade. After conversations,  the nasty things are solved. 

This is the very first class of my computer graphics where the course teacher started from the color mood. How the number of colors is created with the limitations of colors. He described two color methods. One is the RGB method and the other is the CYN method. 

When I returned home I also studied the bias theorem. Bias theorems work in conditional probability. After that,  I created a method in my app by which I can find my current location that returns the latitude and longitude for a particular area. Also, I can transfer the data from one page to another page. 

`dart code of geolocator`

```dart
 import 'package:geolocator/geolocator.dart'; 
Future<Position?> determinePosition() async {
  LocationPermission permission;
  permission = await Geolocator.checkPermission();
  if (permission == LocationPermission.denied) {
    permission = await Geolocator.requestPermission();
    if (permission == LocationPermission.deniedForever) {
      return Future.error('Location Not Available');
    }
  }
  return await Geolocator.getCurrentPosition();
}
```

```dart
import 'dart:convert';
import 'package:http/http.dart' as http;
import '../model/model_data.dart';

class WeatherAPiLatLonPass {
  Future<Weather>? getCurrentWeatherInfoLatLon(
      dynamic lati, dynamic loni) async {
    var api = "74e7c3a1e8f06f40b24cc4a81b032d3*"; 
        // * is alphbet
    var endpoint = Uri.parse(
        "https://api.openweathermap.org/data/2.5/weather?lat=$lati&lon=$loni&appid=$api&units=metric");

    var response = await http.get(endpoint);

    var body = jsonDecode(response.body);

    Weather weather = Weather.fromJson(body);

    //print("-----------------\n"); print(weather.cityName);print(body);
    return weather;
  }
}
```

## Jan - 31 :

I woke up at 9:22 am when my bus is at 10:00 am. I took a quarter minute to prepare as I caught the bus on time.  Alhamdulillah, I catch the bus successfully and I take my morning tea cup from the university cafeteria. And,  I went to the class of VLSI where the teacher discussed a lot of terms about VLSI. 

First, start the lecture from FET and types. How does it work?   He mainly focused on n-channel actions. By this, we know how actual current and voltage pass through the channel. 

We also have a class on Software Engineering, but the teacher is back-to-back and misses the class. Noting so far learn where 2 weeks have already gone.

I also met with my ex-roommate who is currently doing a job in my college in the same department. We discuss some internal issues about the college along with his research defense. 

Though my class is canceled, I am trying to talk with my co-supervisor about the third-year project. We started the conversation about our progress and at that time another teacher arrived and closed our meeting. What the hell,  I felt a little more depressed. I am also concerned about submitting the assignment.

## Feb - 01

I went to Lu like on other days. In the morning Summon took a class about web development from w3school. I do not support his teaching method or the System of my college. I think they should rearrange the educational system, particularly in CSE. 

We started learning elementary HTML. In HTML, it is divided into two portions. One is &lt;head&gt; &lt;/head&gt;  and another is &lt; body &gt; &lt;/body&gt; 

We took store meta information in the head tag, wherein in the body tag we put all attributes and elements that we want to see on our web page.

After that, there had no class. When I return, I met with my friends for making a plan to visit Jaflong once again. We spent a lot of time arranging this party.

## Feb - 02

I woke up too early and reach the bus station where my colleagues waiting for me. For the last time, we checked whether everyone come or not and whether the necessary things store on the bus.

From starting the bus to the spot I enjoyed every minute with my friends. 

In the afternoon I back to the city and bought flowers for decorating my friend's home. As his marriage is the after I go to my friend's home and we enjoyed much 

No learning this day.

### **Feb - 03**

I am back in the city for her birthday. Before I joined her party, I write code in a flutter that dynamically catch the location of the user. 

This code works perfectly but when I am trying to merge but it gives an error. 

After that, I am going to where there she is waiting for me. Moreover, we celebrate the day and ordered heavy food. When I return home I got tired, but I am trying to solve my problem but I could not fix it. 

No major learning this day. 

## **Feb - 04**

I woke up at 10:00 clock to call Galib. But already I miss the college bus. I am going to college locally. This is very humdrum for me to follow the way.

In my computer graphics lab, I learned how to install graphics. h in code blocks. In the computer, everything works according to the pixel. I drew some lines by x1 and x2. 

After that, I have web lab, but no major improvement in this class. Moreover, we again met with our co-advisor to review our app. He saw it and said nothing is an improvement. 

When I return home I tried to pass data from my app to firebase but I am a failure. Bu continues to the trying. 

## **Feb - 05**

I am trying to pass data from my app to flutter but I am failing. I mark some things that how to data retrieve data from cloud storage to the app. 

After that, I again write a code for my weather project where I am trying to add a careful message through the weather status code. 

```dart
"weather": [ 
  { 
    "id": 500,
    "main": "Rain", 
    "description": "light rain",
    "icon": "10n"
  }
]
```

  
I am unable to this code to convert in JSON. I am trying to google but I could not find the way. I searched on the CHAT-GPT it gives me the answer within very few minutes. The power of AI.

This is very simple but I could not think of it before seeing the result.

```dart
id = json['weather'][0]['id'];
```

I spent most of my time on flutter backend works though I do not reach the goal I have familiar with many terms.

This is all for this week. Thank you and see you next week.