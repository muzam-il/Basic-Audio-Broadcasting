# Open Live Voice Only for Android

*其他语言版本： [简体中文](README.zh.md) | [English](README.md) | [മലയാളം](README.ml.md)*

Agora വോയ്‌സ് SDK ഉപയോഗിച്ച് നിങ്ങളുടെ Android അപ്ലിക്കേഷനുകളിലേക്ക് തത്സമയ വോയ്‌സ് പ്രക്ഷേപണം സംയോജിപ്പിക്കാൻ സഹായിക്കുന്ന ഒരു ഓപ്പൺ സോഴ്‌സ് ഡെമോയാണ് Android സാമ്പിൾ അപ്ലിക്കേഷനായുള്ള ഓപ്പൺ ലൈവ് വോയ്‌സ്.

ഈ സാമ്പിൾ അപ്ലിക്കേഷൻ ഉപയോഗിച്ച്, നിങ്ങൾക്ക് കഴിയും:

-ചാനലിൽ ചേരുക / ഉപേക്ഷിക്കുക
- ബ്രോഡ്‌കാസ്റ്റർ അല്ലെങ്കിൽ ശ്രവണമായി റോൾ സജ്ജമാക്കുക
- ഓഡിയോ നിശബ്ദമാക്കുക / നിശബ്ദമാക്കുക
- സ്പീക്കർ സ്വിച്ചുചെയ്യുക

ഒരു ട്യൂട്ടോറിയൽ ഡെമോ ഇവിടെ കാണാം: [Agora-Android-Voice-Tutorial-1to1](https://github.com/AgoraIO/Basic-Audio-Call/tree/master/One-to-One-Voice/Agora-Android-Voice-Tutorial-1to1)


## അപ്ലിക്കേഷൻ പ്രവർത്തിപ്പിക്കുന്നു
**ആദ്യം**, ഒരു ഡവലപ്പർ അക്കൗണ്ട് സൃഷ്ടിക്കുക: [Agora.io](https://dashboard.agora.io/signin/), App ID നേടുക. നിങ്ങളുടെ അപ്ലിക്കേഷൻ ഐഡി ഉപയോഗിച്ച് "app/src/main/res/values/strings_config.xml" അപ്‌ഡേറ്റ് ചെയ്യുക.

```
<string name="private_app_id"><#YOUR APP ID#></string>
```
**അടുത്ത ഘട്ടം**, Agora Voice SDK സമന്വയിപ്പിക്കുക, സംയോജിപ്പിക്കാൻ രണ്ട് വഴികളുണ്ട്:

- സംയോജിപ്പിക്കുന്നതിനുള്ള ശുപാർശിത മാർഗം:

അഗോറ വോയ്‌സ് എസ്‌ഡികെ സ്വപ്രേരിതമായി Jceneter വഴി സമന്വയിപ്പിക്കാൻ കഴിയുന്ന വിലാസം ചേർക്കുക "app/build.gradle":

```
implementation 'io.agora.rtc:voice-sdk:2.4.0'
```

(ഈ സാമ്പിൾ പ്രോഗ്രാം ഈ വിലാസം ചേർത്തു, വീണ്ടും ചേർക്കേണ്ട ആവശ്യമില്ല. നിങ്ങളുടെ സ്വന്തം ആപ്ലിക്കേഷനിൽ Agora voice SDK വേണമെങ്കിൽ ലിങ്ക് വിലാസം ചേർക്കുന്നത് ഏറ്റവും പ്രധാനപ്പെട്ട ഘട്ടമാണ്.)

-സംയോജിപ്പിക്കുന്നതിനുള്ള ഇതര മാർഗം:

ആദ്യം, **Agora Voice SDK** ഇതിൽ നിന്ന് ഡൗൺലോഡുചെയ്യുക  [Agora.io SDK](https://www.agora.io/en/download/). ഡൗൺലോഡ്ചെയ്‌ത SDK പാക്കേജ് അൺ‌സിപ്പ് ചെയ്ത് പകർ‌ത്തുക ***.jar** under **libs** to **app/libs**, **arm64-v8a**/**x86**/**armeabi-v7a** under **libs** to **app/src/main/jniLibs**.

Then, add the fllowing code in the property of the dependence of the "app/build.gradle":

```
compile fileTree(dir: 'libs', include: ['*.jar'])
```

**Finally**, open project with Android Studio, connect your Android device, build and run.

Or use `Gradle` to build and run.

## Developer Environment Requirements
- Android Studio 3.0 or above
- Real devices (Nexus 5X or other devices)
- Some simulators are function missing or have performance issue, so real device is the best choice

## Connect Us
- You can find full API document at [Document Center](https://docs.agora.io/en/)
- You can file bugs about this demo at [issue](https://github.com/AgoraIO/Basic-Audio-Broadcasting/issues)

## License
The MIT License (MIT).
