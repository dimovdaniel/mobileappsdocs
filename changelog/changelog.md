# Apps changelog

## 2.1.1 - 2021-06-01

This is a minor version with some small bug fixes on add to cart button in the Client app and the way AppCenter.ms is handling the build. The rename package is not working ok in Appcenter.ms for iOS. So that is why you need to do the iOS name change before you publish the repository.   
  
There is a new Environment variable required

c - android or ios

If APP\_PLATFORM is android then app renaming will be done for android in AppCeneter.ms

Changed files

screens/Items.js  
screens/Item.js  
appcenter-pre-build.sh



## 2.1.0 - 2021-03-18

This is a major update. We have changes more files, so it is recommended to download the new source code and use your can reuse your old config.json file. 

## 2.0.3 - 2021-03-01

This is a minor update, with fixes for fix for prices in item description. Here is a list of the [updated files](https://gist.github.com/dimovdaniel/46bfe58ee86acb694d456e1e2153edce).

To update, either use the new files from CodeCanyon or copy-paste the new/updated files. \( Only screens/Item.js \)

[https://gist.github.com/dimovdaniel/46bfe58ee86acb694d456e1e2153edce](https://gist.github.com/dimovdaniel/46bfe58ee86acb694d456e1e2153edce)

## 2.0.2 - 2021-02-07

This is a minor update, with fixes for ios pod lock file and fixes for images not showing. Here is a list of the [updated files](https://gist.github.com/dimovdaniel/31ba66bfc1a23373b59104f30e5ad387).

To update, either use the new files from CodeCanyon or copy-paste the new/updated files.

## 2.0.1 - 2021-01-27

This is a minor update, with fixes for android build only. Here is a list of the [updated files](https://gist.github.com/dimovdaniel/3ba74ff31d44db3b3813ad119079d881).

To update, either use the new files from CodeCanyon or copy-paste the new/updated files.  
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

* Fixed ios build 

## 1.2.0 - 2020-05-26

### Initial

* Initial version

