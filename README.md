[![](https://jitpack.io/v/mahmoudramzy400/custom-uvc-android.svg)](https://jitpack.io/#mahmoudramzy400/custom-uvc-android)

CustomUVCAndroid
=========

Library and sample to access UVC camera on non-rooted Android device


How do I use it?
---

### Setup


R8 / ProGuard
-------------

If you are using R8 the shrinking and obfuscation rules are included automatically.

ProGuard users must manually add the below options.
```groovy
-keep class com.herohan.uvcapp.** { *; }
-keep class com.serenegiant.usb.** { *; }
-keepclassmembers class * implements com.serenegiant.usb.IButtonCallback {*;}
-keepclassmembers class * implements com.serenegiant.usb.IFrameCallback {*;}
-keepclassmembers class * implements com.serenegiant.usb.IStatusCallback {*;}
```

Requirements
--------------
Android 5.0+