# OneSignal Push notification

You can follow this guide by OneSignal to enable Push Notifications in the Android and iOS apps. Note that OneSignal is not set via AppCenter.ms since there are manual steps that you need to configure in order to make the push work on iOS.

{% embed url="https://documentation.onesignal.com/docs/react-native-sdk-setup" %}

You should be able to register multiple apps on a single OneSignal App. Since in OneSignal you don't set the app id, but rather the Firebase Setup for Android  and p12 certificate for ios.

In Firebase register all your apps under one firebase instance. 

On iOS bundle all your apps with the same push identifier. 

