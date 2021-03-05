This build represents an unofficial fork of the recently open sourced Waveform Synthesizer Vital, which includes modifications to the `jucer` and `make` files as well as other parts of the source to successfully build Vitalium as


 - a Standalone app with JACK support
 - a VST3 plugin
 - LV2 plugin 

for Linux/GNU. 

The changes that are integrated into this build include crucial fixes that were implemented by 


 - falkTX (removing of all the Log In, Authorization,Downloading of Content and Text-to-Wavform features both in the GUI and in the back end) 
 - taylordotfish (LV2 fixes to enable the GUI to display) 


Successfully tested and built on Debian Buster. 

instructions

```
git clone https://github.com/tank-trax/vitalium.git
cd vitalium
make
```

This will produce the Standalone and VST3 in `vitalium/plugin/builds/linux_vst/build/` and the LV2 in `vitalium/plugin/builds/linux_lv2/` 

I have made every effort to comply with Matt's wishes to remove all mention of "Vital", "Vital Audio", "Tytel" or "Matt Tytel" from the jucer, Makefile and all source code as well as take away any mention of or link to https://vital.audio, https://account.vital.audio or https://store.vital.audio


## What can you do with the source
The source code is licensed under the GPLv3. If you download the source or create builds you must comply with that license.

### Things you can't do with this source
 - Do not create an app and distribute it on the iOS app store. The app store is not comptabile with GPLv3 and you'll only get an exception for this if you're paying for a GPLv3 exception for Vital's source (see Code Licensing above).
 - Do not use the name "Vital", "Vital Audio", "Tytel" or "Matt Tytel" for marketing or to name any distribution of binaries built with this source. This source code does not give you rights to infringe on trademarks.
 - Do not connect to any web service at https://vital.audio, https://account.vital.audio or https://store.vital.audio from your own builds. This is against the terms of using those sites.
```
