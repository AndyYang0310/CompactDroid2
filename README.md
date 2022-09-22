# CompactDroid Overview
We propose an app Constraint Analysis approach named CompatDroid to select the optimal device to guide crowd testers. CompatDroid only needs no more than 7 Android versions to achieve almost the same code coverage testing on all 14 android versions in 36 of 46 apps. It can drastically reduce the consumption of test resources while losing little test coverage for crowdtesting.

![overview](https://user-images.githubusercontent.com/107869122/191693701-892c3c46-e8b7-43eb-b8e7-4ec1f96e2a31.png)

# Environment Configration
* Ubuntu 20.04
* Java: 1.8
* Android SDK: API 20+

Run CompactDroid
```
./run.sh $apk
```
$apk indicates the app to run.

#Constraints list

```
public class Build {
    method public static java.lang.String getRadioVersion();
    method public static java.lang.String getSerial();
    field public static final java.lang.String BOARD;
    field public static final java.lang.String BOOTLOADER;
    field public static final java.lang.String BRAND;
    field public static final deprecated java.lang.String CPU_ABI;
    field public static final deprecated java.lang.String CPU_ABI2;
    field public static final java.lang.String DEVICE;
    field public static final java.lang.String DISPLAY;
    field public static final java.lang.String FINGERPRINT;
    field public static final java.lang.String HARDWARE;
    field public static final java.lang.String HOST;
    field public static final java.lang.String ID;
    field public static final java.lang.String MANUFACTURER;
    field public static final java.lang.String MODEL;
    field public static final java.lang.String PRODUCT;
    field public static final deprecated java.lang.String RADIO;
    field public static final deprecated java.lang.String SERIAL;
    field public static final java.lang.String[] SUPPORTED_32_BIT_ABIS;
    field public static final java.lang.String[] SUPPORTED_64_BIT_ABIS;
    field public static final java.lang.String[] SUPPORTED_ABIS;
    field public static final java.lang.String TAGS;
    field public static final long TIME;
    field public static final java.lang.String TYPE;
    field public static final java.lang.String UNKNOWN = "unknown";
    field public static final java.lang.String USER;
  }

  public static class Build.VERSION {
    ctor public Build.VERSION();
    field public static final java.lang.String BASE_OS;
    field public static final java.lang.String CODENAME;
    field public static final java.lang.String INCREMENTAL;
    field public static final int PREVIEW_SDK_INT;
    field public static final java.lang.String RELEASE;
    field public static final deprecated java.lang.String SDK;
    field public static final int SDK_INT;
    field public static final java.lang.String SECURITY_PATCH;
  }
```
