This build represents my personal modifications to the jucer file within the plugin folder to successfully build Vitalium Standalone with JACK support and the VST3 plugin. A

This has been tested and built successfully on Debian Buster, but it should build on any Linux distribution

instructions

```
git clone https://github.com/tank-trax/vitalium.git
cd vitalium
git checkout vitalium-1.0.6
cd plugin/builds/linux_vst/
make CONFIG=Release
```

this will build the Standalone and VST3

I have made every attempt to comply with Matt's wishes to remove all mention of "Vital", "Vital Audio", "Tytel" or "Matt Tytel" from the jucer and Makefile as well as take away any mention of or link to https://vital.audio, https://account.vital.audio or https://store.vital.audio

The "Check for Updates" section has been removed from the About screen.

## What can you do with the source
The source code is licensed under the GPLv3. If you download the source or create builds you must comply with that license.

### Things you can't do with this source
 - Do not create an app and distribute it on the iOS app store. The app store is not comptabile with GPLv3 and you'll only get an exception for this if you're paying for a GPLv3 exception for Vital's source (see Code Licensing above).
 - Do not use the name "Vital", "Vital Audio", "Tytel" or "Matt Tytel" for marketing or to name any distribution of binaries built with this source. This source code does not give you rights to infringe on trademarks.
 - Do not connect to any web service at https://vital.audio, https://account.vital.audio or https://store.vital.audio from your own builds. This is against the terms of using those sites.
