This build represents my personal modifications to the jucer file and parts of the source to successfully build Vitalium Standalone with JACK support and the VST3 plugin for Linux. The VST2 portion has been removed and there has been no attempt at modifying the LV2. I did try to build the LV2 and got as far as it loaded in jalv.gtk3 but without any GUI. 

These modifications have been tested and built successfully on Debian Buster, and should build on any Linux distribution. 

instructions

```
git clone https://github.com/tank-trax/vitalium.git
cd vitalium
git checkout vitalium-1.0.6
cd plugin/builds/linux_vst/
make CONFIG=Release
```

I have made every attempt to comply with Matt's wishes to remove all mention of "Vital", "Vital Audio", "Tytel" or "Matt Tytel" from the jucer and Makefile as well as take away any mention of or link to https://vital.audio, https://account.vital.audio or https://store.vital.audio

Small tweaks include the "Check for Updates" section has been removed from the About screen and the "Download Content" button  has been removed from the Pop-up window.

If any one would like to contribute to this build in a graphic design capacity (to change the allure or skin so that is is unique from Vital) I would welcome such changes with enthusiasm.

## What can you do with the source
The source code is licensed under the GPLv3. If you download the source or create builds you must comply with that license.

### Things you can't do with this source
 - Do not create an app and distribute it on the iOS app store. The app store is not comptabile with GPLv3 and you'll only get an exception for this if you're paying for a GPLv3 exception for Vital's source (see Code Licensing above).
 - Do not use the name "Vital", "Vital Audio", "Tytel" or "Matt Tytel" for marketing or to name any distribution of binaries built with this source. This source code does not give you rights to infringe on trademarks.
 - Do not connect to any web service at https://vital.audio, https://account.vital.audio or https://store.vital.audio from your own builds. This is against the terms of using those sites.
