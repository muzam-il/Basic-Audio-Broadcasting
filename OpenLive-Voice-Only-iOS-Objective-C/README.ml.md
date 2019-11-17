# iOS Objective C യ്ക്കായി മാത്രം തത്സമയ ശബ്‌ദം തുറക്കുക

*[简体中文](README.zh.md) | [English](README.md) | [മലയാളം](README.ml.md)*

Agora Voice SDK ഉപയോഗിച്ച് നിങ്ങളുടെ iOS അപ്ലിക്കേഷനുകളിലേക്ക് തത്സമയ വോയ്‌സ് ചാറ്റ് സംയോജിപ്പിക്കാൻ സഹായിക്കുന്ന ഒരു ഓപ്പൺ സോഴ്‌സ് ഡെമോയാണ് objective C സാമ്പിൾ അപ്ലിക്കേഷനായി ഓപ്പൺ ലൈവ് വോയ്‌സ് iOS.

ഈ സാമ്പിൾ അപ്ലിക്കേഷൻ ഉപയോഗിച്ച്, നിങ്ങൾക്ക് കഴിയും:

-ചാനലിൽ ചേരുക / ഉപേക്ഷിക്കുക
- ബ്രോഡ്‌കാസ്റ്റർ അല്ലെങ്കിൽ ശ്രവണമായി റോൾ സജ്ജമാക്കുക
- ഓഡിയോ നിശബ്ദമാക്കുക / നിശബ്ദമാക്കുക
- സ്പീക്കർ സ്വിച്ചുചെയ്യുക

ഒരു ട്യൂട്ടോറിയൽ ഡെമോ ഇവിടെ കാണാ: [Agora-iOS-Voice-Tutorial-Swift-1to1](https://github.com/AgoraIO/Basic-Audio-Call/tree/master/One-to-One-Voice/Agora-iOS-Voice-Tutorial-Swift-1to1)

## Running the App
**ആദ്യം**, ഒരു ഡവലപ്പർ അക്കൗണ്ട് സൃഷ്ടിക്കുക: [Agora.io](https://dashboard.agora.io/signin/), App ID നേടുക.നിങ്ങളുടെ അപ്ലിക്കേഷൻ ഐഡി ഉപയോഗിച് "AppID.m" അപ്‌ഡേറ്റ് ചെയ്യുക.

```
return "YOUR APPID"
```

ആദ്യം, **Agora Voice SDK** ഇതിൽ നിന്ന് ഡൗൺലോഡുചെയ്യുക [Agora.io SDK](https://www.agora.io/en/blog/download/). ഡൗൺലോഡ്ചെയ്‌ത SDK പാക്കേജ് അൺ‌സിപ്പ് ചെയ്ത് പ്രോജക്റ്റിലെ ഫോൾഡർ "OpenLive-Voice-Only-iOS-Objective-C" ലേക്ക് പകർ‌ത്തുക **libs/AgoraAudioKit.framework**.

Finally, Open OpenLive-Voice-Only-iOS-Objective-C.xcodeproj, connect your iPhone／iPad device, setup your development signing and run.

## Developer Environment Requirements
* XCode 8.0 +
* Real devices (iPhone or iPad)
* iOS simulator is NOT supported

## Connect Us

- You can find full API document at [Document Center](https://docs.agora.io/en/)
- You can file bugs about this demo at [issue](https://github.com/AgoraIO/Basic-Audio-Broadcasting/issues)

## License

The MIT License (MIT).
