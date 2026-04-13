# Journal Entries
## April 12th, 2026 - Sunday
Every time I solder, I find myself inhaling the fumes that come from flux. From my research, inhaling too much flux can lead to respiratory problems in the future. To keep myself alive for a few extra years, I want to have something that draws the fumes away from me. 

On Amazon, there are fume extractors for 40+ dollars. I don't have that kind of money, so I can design one myself based off of their designs. Their designs seem quite simple, a fan pulls air into a filter. However, they don't have all the features I want, especially for 40 dollars. 

### Deciding on Parts
Here's a list of everything I want in my fume extractor
1. Filter
    - Kind of a no brainer, I don't want for the fumes to linger after I've pulled it away
2. Speed Control
    - To control the speed
3. OLED Screen
    - It'll tell me what fan speed I'm running at
4. A Case
    - It'll look better and neat with a case.
5. USB-C input
    - It'll be easier to power

I think thats it! Time to start the BOM and design. 

For the fan, I'll use an old 120mm PC fan I have at home. It takes 12v of power and 5v for it's digital signal. 

To filter the air, I'll use a combination of a HEPA filter and a carbon filter. Most fume extractors on Amazon only have a carbon filter. HEPA filters capture other pollutants that carbon filters don't capture. 

To control the speed, I'll use a combination of a rotary encoder, OLED screen, and an Arduino Nano. I want to use a rotary encoder because I already have one and I can click to set speed. I'll use a 0.91in OLED Screen because it's not too big but big enough to show the rpm of the fan. The Arduino can read the RPM of the fan with the fan's tachometer. However, since the fan takes 

I can 3D print a custom case easily. This ensures that my final product can look nice. 

I want to use USB-C instead of a barrel jack because I hate barrel jacks. I don't get why there's a hundred different sizes and each size has two polarities. I love how USB-C is a universally agreed on port.

### Sourcing Parts
When sourcing parts, I'm looking for the cheapest and smallest options on the market.

1. HEPA Filter
    I found somebody who made a 120mm fan attachment. They used [these](https://www.aliexpress.us/item/2251832851641089.html).
2. Carbon Filter
I just found [these](https://www.aliexpress.us/item/3256808473751203.html) that were ordered a ton on AliExpress.
3. OLED Screen
    https://www.aliexpress.us/item/3256808590741849.html
4. Buck Converter
    I found [this one](https://www.aliexpress.us/item/3256807183204284.html) with a relatively small form factor. It steps down from 12v to 5v, perfect for what I need
5. USB-C
    Great Scott covered [these](https://www.aliexpress.us/item/3256805275538893.html) in one of these videos. They honestly look amazing and I know exactly how I'll incorporate it into this project.
    ![image](/journal/assets/USBC_1.png)

I think that's it! I'll create the full BOM right now and I should be able to start 3D modeling the case. 
![image](/journal/assets/BOM.png)
Is it over 40 dollars? Yes. Is it cooler than a 40 dollar one? Yes. I also own most of the parts already. After subtracting everything, it'll only cost me $26.43 USD. It also comes with extra parts. Since it's getting late and I have school tomorrow, I'll model the case tomorrow. 

For now, I'll just work on organizing this repository.

## April 13th, 2026 - Monday
After rewatching the USB-C port segment on Great Scott's youtube video, I found out that I'll need resistors to pull the correct current from the power supply. However, on doing more research, using resistors only supplies 5v. To get 12v, I'll need a USB C decoy module. 

Unfortunately, all the USB-C ports with the mounting plates don't have a PD chip, so I'll have to buy one without a mounting plate. 

I found this one!

https://www.aliexpress.us/item/3256810424345892.html

It has a small footprint so it shouldn't bulk up my fume extractor too much.
