This build represents an unofficial fork of the recently open sourced Waveform Synthesizer Vital, which includes modifications to the `jucer` and `make` files as well as other parts of the source code to successfully build "Vitality +/-" for Linux/GNU as:


 - Standalone app with JACK support
 - VST3 plugin
 - LV2 plugin 

This build changes the file name(s) and folder location for presets and settings so as to not conflict with the upcoming DISTRHO-Ports Community Build.

Changes integrated into this build include critical fixes implemented by:

 - falkTX (removing the Log In, Authorization, Downloading of Content and Text-to-Waveform features) 
 - taylordotfish (LV2 fixes to enable the GUI to display) 

This build has been successfully tested and built on Debian Buster and should build on an Linux distribution with the requisite development files and libraries.

Instructions

```
git clone https://github.com/tank-trax/vital.git
cd vital
git checkout vitality+minus-1.0.6
make
```

This will produce the Standalone and VST3 in `plugin/builds/linux_vst/` and the LV2 in `plugin/builds/linux_lv2/` 

Presets and local store will go in the `~/.local/share/vitality+minus/` folder

I have made every effort to comply with Matt's wishes to remove all mention of "Vital", "Vital Audio", "Tytel" or "Matt Tytel" from the jucer, Makefile and all source code as well as take away any mention of or link to https://vital.audio, https://account.vital.audio or https://store.vital.audio


## What can you do with the source
The source code is licensed under the GPLv3. If you download the source or create builds you must comply with that license.

### Things you can't do with this source
 - Do not create an app and distribute it on the iOS app store. The app store is not comptabile with GPLv3 and you'll only get an exception for this if you're paying for a GPLv3 exception for Vital's source (see Code Licensing above).
 - Do not use the name "Vital", "Vital Audio", "Tytel" or "Matt Tytel" for marketing or to name any distribution of binaries built with this source. This source code does not give you rights to infringe on trademarks.
 - Do not connect to any web service at https://vital.audio, https://account.vital.audio or https://store.vital.audio from your own builds. This is against the terms of using those sites.
 - Do not distribute the presets that come with the free version of Vital. They're under a separate license that does not allow redistribution.
```
