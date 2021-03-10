This build represents an unofficial fork of the recently open sourced Waveform Synthesizer Vital, which includes modifications to the `jucer` and other parts of the source code to successfully build "Vitality +/-" for 64 bit Windows using Visual Studio 2017 with ASIO support:

 - Standalone with ASIO
 - VST3 plugin
 - VST2 plugin

This branch is for those that have the VST2_SDK and want to build the VST2 plugin. You will also need the ASIO SDK available at https://new.steinberg.net/developers/ 

Changes integrated into this build include critical fixes implemented by:

 - falkTX (removing the Log In, Authorization, Downloading of Content and Text-to-Waveform features) 

Successfully tested and built on Windows 10 using Visual Studio Community 2017. The only caveat is that IPP (Intel Performance Primitives) needs to be installed.

Instructions

```
git clone https://github.com/tank-trax/vital.git
cd vital
git checkout vitality+-1.0.6-win
```
The build will look in `third_party\VST_SDK\` for ASIO and VST2 headers. Create the folders `third_party\VST_SDK\ASIO_SDK` and `third_party\VST_SDK\VST2_SDK` and place the requisite SDK in each folder.

Open the Solution Visual Studio 2017 and build the Release

This will produce the Standalone and VST3 in `plugin\builds\vs17\x64\Release`

Presets and local store will go in the `Documents\Vitality+Minus` folder

I have made every effort to comply with Matt's wishes to remove all mention of "Vital", "Vital Audio", "Tytel" or "Matt Tytel" from the jucer, Makefile and all source code as well as take away any mention of or link to https://vital.audio, https://account.vital.audio or https://store.vital.audio

## What can you do with the source
The source code is licensed under the GPLv3. If you download the source or create builds you must comply with that license.

### Things you can't do with this source
 - Do not create an app and distribute it on the iOS app store. The app store is not comptabile with GPLv3 and you'll only get an exception for this if you're paying for a GPLv3 exception for Vital's source (see Code Licensing above).
 - Do not use the name "Vital", "Vital Audio", "Tytel" or "Matt Tytel" for marketing or to name any distribution of binaries built with this source. This source code does not give you rights to infringe on trademarks.
 - Do not connect to any web service at https://vital.audio, https://account.vital.audio or https://store.vital.audio from your own builds. This is against the terms of using those sites.
 - Do not distribute the presets that come with the free version of Vital. They're under a separate license that does not allow redistribution.
```
