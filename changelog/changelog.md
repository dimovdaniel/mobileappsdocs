# 📅 Apps changelog

## 3.6.1 - 2022-11-12 - WhatsApp Taxi App update

This is a small update only for WhatsApp Driver Taxi App.&#x20;

It brings the possibility to send live tracking links to the client

Add the message in /constants/Language.js

```
message_when_approved_tracking: "Here, You can track my current location here ->",
```

The only change is in  /screens/OrderDetails.js around line 247

```javascript
if(issd){
   var approveMessage=Language.message_when_approved;
   //Append the location tracking option
   approveMessage+="\n\n"+Language.message_when_approved_tracking+"\n\n"+config.domain+"/l/"+order.md;
   sendWhatsAppMessage(approveMessage);
}
```

{% embed url="https://share.cleanshot.com/XvTS2p" %}

## 3.6.0 - 2022-08-25

In this version we have updated the mobile app code to use expo 46 (the latest at the moment).&#x20;

We did that because, in expo 44, apps are compiled with android SDK 30, and google now requires android SDK 31.&#x20;

We had to use a new module for the Toast, so now the toast notification will look a bit better.&#x20;

In order to update from 3.5.0 we will suggest starting fresh with the new source code and copying the existing config.js and app.json content and the resources you have in the assets folder.

<figure><img src="../.gitbook/assets/CleanShot 2022-08-25 at 17.58.35.png" alt=""><figcaption></figcaption></figure>

## 3.5.0 - 2022-08-15

In this version, you have the option to deactivate user account directly from the mobile app.&#x20;

There are also some other small bug fixes and version bumps.&#x20;

**Update files**

![](../.gitbook/assets/mobile\_app\_3\_5.png)

## 3.2.0 - 2022-03-03

This is another major change to the mobile app.&#x20;

Before we were using Expo bare workflow and was really difficult to configure and publish the app. &#x20;

We moved to expo-managed workflow. This makes the building and submitting process so much easier.  We have removed Onesignal native SDK, and instead, we use Expo Push notifications.

Mobile apps are compatible with older versions of the web project, but in order to have expo push, you need web version 3.2.0+&#x20;

**How to update your previous app.**

In case you already have a working mobile app code, there is not much to reuse. But the setup in config.js is relatively simple. ( don't do copy-paste  of config.js since the format is changed now )

**If you already have an app on google play and the app store**

In that case, you need to enter the same bundle identifier (iOS)  / package name (android) and use your local keystore (  android ).&#x20;



## 3.0.0 - 2021-08-16

This is a major update. We have changes more files, so it is recommended to download the new source code and use your can reuse your old config.json file.

In this update we have removed the Stripe SDK. This SDK was outdated, and google started rejecting apps because of it.

This update also uses the latest ReactNative navigation, and expo SDK.

It is important if you use the Client Mobile app, to use the latest version of the FoodTiger web project. Since from this version on, the list of payment methods is returned from the web api.

## 2.1.1 - 2021-06-01

This is a minor version with some small bug fixes on add to cart button in the Client app and the way AppCenter.ms is handling the build. The rename package is not working ok in Appcenter.ms for iOS. So that is why you need to do the iOS name change before you publish the repository.

There is a new Environment variable required

**APP\_PLATFORM** - **android** or **ios**

If **APP\_PLATFORM** is android then app renaming will be done for android in AppCeneter.ms

Changed files

screens/Items.js\
screens/Item.js\
appcenter-pre-build.sh

## 2.1.0 - 2021-03-18

This is a major update. We have changes more files, so it is recommended to download the new source code and use your can reuse your old config.json file.

## 2.0.3 - 2021-03-01

This is a minor update, with fixes for fix for prices in item description. Here is a list of the [updated files](https://gist.github.com/dimovdaniel/46bfe58ee86acb694d456e1e2153edce).

To update, either use the new files from CodeCanyon or copy-paste the new/updated files. ( Only screens/Item.js )

[https://gist.github.com/dimovdaniel/46bfe58ee86acb694d456e1e2153edce](https://gist.github.com/dimovdaniel/46bfe58ee86acb694d456e1e2153edce)

## 2.0.2 - 2021-02-07

This is a minor update, with fixes for ios pod lock file and fixes for images not showing. Here is a list of the [updated files](https://gist.github.com/dimovdaniel/31ba66bfc1a23373b59104f30e5ad387).

To update, either use the new files from CodeCanyon or copy-paste the new/updated files.

## 2.0.1 - 2021-01-27

This is a minor update, with fixes for android build only. Here is a list of the [updated files](https://gist.github.com/dimovdaniel/3ba74ff31d44db3b3813ad119079d881).

To update, either use the new files from CodeCanyon or copy-paste the new/updated files.\
Remove the node\_modules and reinstall again.

## 2.0.0 - 2021-01-22

This is a major update. We have updated all the core plugins we use and made the project works with the latest Foodtiger API.

### New

* MiltiCity
* Item variants and extras
* Payment via PayPal, Mollie, PayStack

In order to update, we recommend starting from scratch. You can reuse your old images etc. And the changing of configuration is relatively easy.

## 1.3.1 - 2020-07-13

### **Fixed**

* Included debug key for android
* Fixes for distribution on android
* Bette docs

## 1.3.0 - 2020-06-05

### Fixed

* Fixed ios build&#x20;

## 1.2.0 - 2020-05-26

### Initial

* Initial version
