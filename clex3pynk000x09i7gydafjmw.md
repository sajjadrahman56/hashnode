---
title: "9th week of 52 weeks"
datePublished: Mon Mar 06 2023 17:33:52 GMT+0000 (Coordinated Universal Time)
cuid: clex3pynk000x09i7gydafjmw
slug: 9th-week-of-52-weeks
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1678123835117/43413131-155c-48f1-9dcf-9d16eedf3c1d.png
tags: machine-learning, beginner, linearregression, 52weeks, sajjadrahman

---

### 28 Feb  to 2 March

* Most of the time I have passed to fix project bugs, write reports, make presentations and meet with my teammates. 
    
* I went to college before the defense day as one of my teammates can have clear ideas about my projects.
    
* I could not complete my project yet but I will continue the further process. 
    
* On the defense day we were very tense, when we did it we felt we released a burden that weight nearly thousands KG.
    
* We took many pictures with our team friends and teachers as our defense was good.
    
* In the evening the college arranged a Gala Night for the very first time. More than 500 folks were participating. We enjoyed every second of that moment and took snaps to make it memorable.
    

### 3 - Mar

As I came back home late at night I woke up in the late morning. I felt uncomfortable, but I am watching some basic tutorials in HTML and CSS. 

As it is Friday, my friend and I visited the nearby eco-park. We talked about Ai and also those people who have no idea about the future of AI. Many of our friends have no proper idea about this.

  
In the evening I have a meeting with the BD SPARK IEEE volunteer team as they recruit volunteers. They asked many questions, and I did well. But I have not returned the email I received yet.

### 4 - Mar  

It is Saturday, and as all classes were canceled I would not have gone to college. Rather I have passed the time by sleeping as I am weak and reading some articles on ML. Most of the time passed without doing anything. 

### 5 - Mar

As I am weak, I woke up late in the morning. I watched 2 videos on youtube about ML that were made by Andrew NG. He is the boss of AI. I fell in love with his lecture.

The things I learned from his lesson that is about 

`Features` 

`Level` 

`Gradient descent` 

`Cost functions of linear` 

Also, I implemented multiple features of Linear Regression with Python with the help of youtube. As the data is limited I have no idea how to dynamically split the data .’

Why data split, well data split for training a model and testing how the model responds.

Here is my code of multiple features of the `Linear Regression`

```python

import pandas as pd
import numpy as np
from sklearn import linear_model


df = pd.read_csv('car_data.txt')
df
# check particular column 
df.experience
# I wanna replace null value with some data so I apply another rules that is I can perform mean or median here 
df.experience.mean()
# # store in variable the median value 

exp_fit = df.experience.median()
exp_fit
# ### I want to fill the with help of df.experience.fillna('pass value')
df.experience = df.experience.fillna(exp_fit)
# #### see the output 
df.experience
df
reg = linear_model.LinearRegression()
# ### dimentations matter
reg.fit(df[['speed','car_age','experience']],df.risk)
reg.predict([[160,10,5]])
# ## coeficient  find 
reg.coef_
# ## Intercept find 
reg.intercept_
# ## Manuale check the output 
(0.33059217*160) + (1.61053246 * 10  ) - ( 5 * 6.20772074 ) + 33.410000910435905

# ******************************* THANK YOU 
```

Here is the Github link

%[https://github.com/sajjad-njr/PY-ML-and-DS/blob/main/multiple-features-LR.md] 

* Give me suggestions
    
* Forgive my mistake
    
* I am @[Sajjad Rahman](@sajjadrahman) currently learning ML and Flutter