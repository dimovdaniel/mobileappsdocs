---
description: To Google play and app store
---

# 🚀 Deploy app

Once you are ready on how you app works you are ready to publish it. This process is really simple with Expo. You need to create a free account.&#x20;

### Check if project is healthy

Execute&#x20;

```
expo doctor
```

If there are problems

```
expo doctor --fix-dependencies
```

### Create build

Full docs [here](https://docs.expo.dev/build/setup/).&#x20;

Execute

```
eas build --platform all
```

### Submit to Google play

Full docs [here](https://docs.expo.dev/submit/android/)

Execute

```
eas submit -p android
```

### Submit to Apple App Store

Full docs [here](https://docs.expo.dev/submit/ios/)

Execute

```
eas submit -p ios
```
