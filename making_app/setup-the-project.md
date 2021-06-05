---
description: To define it as your own project
---

# Setup the project

Download the Client app source code from CodeCanyon and extract it.  
Open the source code in your favorite text/code editor. We suggest [Visual Studio Code](https://code.visualstudio.com/).

There you will find the file **config.js**

Replace the values with your real values, like the ULR link, desired currency. You should have the same values as in your .env file in FoodTiger web.

### The things you need to change

{% hint style="success" %}
**exports.domain** - with your real domain ending in /api/v2   
  
example.

"exports.domain = "[https://restotiger.com/api/v2](https://restotiger.com/api/v2)";
{% endhint %}

{% hint style="success" %}
**exports.LOGO=**"https://site.com/image.png"; -- Link to your logo/icon \( 1024 x 1024 \)

IMPORTANT -- THIS NEEDS TO BE .**PNG** image. If you use JPEG the process will resut in error.
{% endhint %}

{% hint style="info" %}
If not vendor app.  
The same **GOOGLE\_API\_KEY** should be put in **android/app/src/main/AndroidManifest.xml**  
You can use the same **GOOGLE\_API\_KEY** as in your web project.
{% endhint %}





