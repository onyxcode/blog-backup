---
title: "How to solve the "not in sync" error on Arduino IDE"
datePublished: Mon Feb 22 2021 17:17:01 GMT+0000 (Coordinated Universal Time)
cuid: cklgue84m007me0s1dp4jgqp5
slug: not-in-sync
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1614013363435/5bhcuH_Lz.jpeg
tags: tutorial, cpp, c, arduino, programming-tips

---

If you've ever coded for an Arduino, you're probably familiar with the Arduino IDE. Is your IDE just not uploading your sketch? Are you getting an error such as this?


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1614013525427/6NaWEQkj2.png)

If so, the fix is quite simple. First, locate the `Tools` section on the top bar of the Arduino IDE.


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1614013862476/muxNYwQ3d.png)


Then, hover over the `Port` option.


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1614013908338/YQM2ySkcW.png)

As you can see here, my Arduino UNO is located on serial port `/dev/ttyACM3`. Let's try uploading the sketch again.


![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1614014106789/eA2dMPle3.png)

The sketch is now uploaded! If you enjoyed this tutorial helpful, like it and share it with a friend!