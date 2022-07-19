# RainbowSpiral
Using the Turtle library to create graphics. In this case, I created a rainbow spiral that gets drawn when ran for about 60 seconds. Enjoy!

```
import turtle
from turtle import *

turtle.title("rainbow spiral")
speed(15)
bgcolor("black")
r,g,b=255,0,0

for i in range(255*2):
    colormode(255)
    if i<255//3:
        g+=3
    elif i<255*2//3:
        r-=3
    elif i<255:
        b+=3
    elif i<255*4//3:
        g-=3
    elif i<255*5//3:
        r+=3
    else:
        b-=3
    fd(50+i)
    rt(91)
    pencolor(r,g,b)

done()
```

<img width="734" alt="Screen Shot 2022-07-19 at 9 23 39 AM" src="https://user-images.githubusercontent.com/66803124/179761646-69654022-0229-4c70-8460-2b1084e54495.png">

