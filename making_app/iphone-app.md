---
description: 'IMPORTANT: Follow this step after you have done all of the previous steps'
---

# iPhone App

## POD install

First, you will need to install the cocoa pods. To do that, navigate to the ios folder and execute pod install

```text
cd ios
pod install
```

As a reference, look at this video. Watch until 4:25

{% embed url="https://youtu.be/RuZlzmix5aw?t=235" caption="" %}

## Run the app on Simulator

Soon as you have installed your pods installed, you can run your app on the simulator.  
To do that, navigate to the project root folder. The execute `npm run ios`

```text
cd ..
npm run ios
```

This should start the app on the simulator

As a reference, look at this video. Watch until the end.

{% embed url="https://youtu.be/RuZlzmix5aw?t=274" caption="" %}

As you can see in the video, I get an error the first time, then run the same command again, and all worked ok. If you run into a problem, run the command again. `npm run ios`. If you still get an error, send us a message of the error that you get in the console.

## Deploy on iTunes Connect

The full guide that we looked into is \( [here](https://instabug.com/blog/how-to-submit-app-to-app-store/) \)

From now on, the deployment is like any other xCode - native iOS project. As said in the requirements, you will need your own iOS developer account.

Open the **.xcworkspace** file that is inside the **ios** folder. Then, in the **Signing & Capabilities** select your account. xCode will automatically make all the required certificates and IDs for you.

![](https://github.com/dimovdaniel/mobileappsdocs/tree/91b841dcb5e9e967963ccae0ad89e944d23a46ba/.gitbook/assets/signing.png)

After this, you will need to create the App Store record in iTunes for this account.

### **Add a new app in App Store connect**

In the App Store Connect dashboard, select My Apps.

Click on the **+** sign in the upper left-hand corner, then **New App**.

To create a new App Store Connect record, you’ll need these details: platform, app name, default language, bundle ID, and SKU. You can’t really change these details later, so be sure of what you enter.

* Use keywords in your app name to optimize for discovery.
* The bundle ID must be an exact match of the bundle identifier in your Xcode project Info.plist file \(in the target’s General &gt; Identity section\).
* The SKU is not visible to users and is up to you to set. It can be an identifier you use in your company or something else that is meaningful for you. Acceptable characters include letters, numbers, hyphens, periods, and underscores, and it must begin with a letter or number.

![](https://github.com/dimovdaniel/mobileappsdocs/tree/91b841dcb5e9e967963ccae0ad89e944d23a46ba/.gitbook/assets/createitunesconnectrecord-e1501675429479.png)

### Upload app

Before you can submit your app for review through App Store Connect, you need to upload the build through Xcode.

1. In Xcode, select **Generic iOS Device** as the deployment target.
2. Choose **Product** from the top menu and click on **Archive**.
3. The Xcode Organizer will launch, displaying any archives you’ve created in the past.
4. Make sure the current build is selected and click on **Upload to App Store** in the right-hand panel.
5. Select your credentials and click **Choose**.
6. In the next window that appears, click on **Upload** in the bottom right-hand corner.

A success message will appear when the upload has completed. Click **Done**.

![Step 1 - Setting Generic iOS Device](https://github.com/dimovdaniel/mobileappsdocs/tree/91b841dcb5e9e967963ccae0ad89e944d23a46ba/.gitbook/assets/generic.png)

![](https://github.com/dimovdaniel/mobileappsdocs/tree/91b841dcb5e9e967963ccae0ad89e944d23a46ba/.gitbook/assets/uploadsuccsessful.png)

### Submit app

After the app is upload to App Store connect, it may take ± 30 min apple to process the upload.

You will need to provide a good description of the app. Don't submit the app if you have only a demo restaurant. Apple may reject for that reason.

You will also need to make good screenshots of the app. In order to run the app on different simulators, look into this guide.

[https://reactnative.dev/docs/running-on-simulator-ios\#specifying-a-device](https://reactnative.dev/docs/running-on-simulator-ios#specifying-a-device)

All the process of submitting in detail is explained here: [https://instabug.com/blog/how-to-submit-app-to-app-store/](https://instabug.com/blog/how-to-submit-app-to-app-store/). You can use it to guide you if you are new to the Apple submitting process.

## Help and problems

If you face any problems, don't hesitate to let us know on our support chat.

{% embed url="https://help.mobidonia.com/\#foodtiger" caption="" %}

