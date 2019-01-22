## React-Native Android Emulator Setup for OS X (Updated 01-22-2019)

Follow these instructions to setup an android emulator on OS X.

1. Navigate to: https://medium.com/pvtl/react-native-android-development-on-mac-ef7481f65e47
1. Do all steps in the article stopping before 4.2, because the `android` cli command is now deprecated
1. Open Android Studio, then:

    ### Android SDK Manager
1. From main Android Studio window Click `Configue` (bottom right) > `SDK Manager`
1. Look at the list under SDK Platforms column
1. Check the box at the bottom right to "Show Package Details"
1. Look for `Android 7.1 (Nougat)`
    * Check the box next to these three packages under `7.1 (Nougat)`:
        - [ ] Android TV Intel x86 Atom System Image
        - [ ] Google APIs Intel x86 Atom 64 System Image
        - [ ] Google APIs Intel x86 Atom System Image
    * Click "`Apply`" button and follow instructions for downloading & installing

1. Look for `Android 6.0 (Marshmallow)` in the list
    * Check the box next to these two packages under `6.0 (Marshmallow)`:
        - [ ] Android SDK Platform 23
        - [ ] Google APIs Intel x86 Atom System Image
    * Click "`Apply`" button and follow instructions for downloading & installing
    * Close the SDK Manager window (hit red X top left)

    ### Android ADV Manager
1. From main Android Studio window Click `Configure` (bottom right) > `ADV Manager`
1. Select `Nexus 5X` from the list
1. Click "`Next`" button
1. Select `Nougat (Android 7.1.1)` from the list
    * Click the blue "`Download`" link if you need to install (if you can't click "`Next`" you will need to install) and follow instructions
1. Click "`Next`" button
1. Click "`Finish`" button

1. Click the triangle shaped `Play/Start button |>` next to your newly created emulator to launch it

1. In the cli, when emulator has fully booted type:
    * `$ npm run android`
