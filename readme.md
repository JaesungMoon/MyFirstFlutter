
home page
https://flutter.dev/

dl link
https://flutter.dev/docs/get-started/install/macos


flutter_macos_v1.2.1-stable


```
cd ~/development
unzip ~/Downloads/flutter_macos_v1.2.1-stable.zip

export PATH="$PATH:`pwd`/flutter/bin"
```
flutter doctor

# Flutter requires Android SDK 28 and the Android BuildTools 28.0.3
# update android sdk

$ /Applications/ADT/sdk/tools/bin/sdkmanager "platforms;android-28" "build-tools;28.0.3"

if it still has issue.
✗ Android license status unknown.

$ flutter doctor --android-licenses
A newer version of the Android SDK is required. To update, run:
/Applications/ADT/sdk/tools/bin/sdkmanager --update

ref url
https://qiita.com/ko2ic/items/8d36bcc50dc62a07936c

# for iOS matter
[!] iOS toolchain - develop for iOS devices (Xcode 10.1)
✗ libimobiledevice and ideviceinstaller are not installed. To install with Brew, run:

$ brew update
$ brew install --HEAD usbmuxd
$ brew link usbmuxd
$ brew install --HEAD libimobiledevice
$ brew install ideviceinstaller

Error: An unexpected error occurred during the `brew link` step
The formula built, but is not symlinked into /usr/local
Permission denied @ dir_s_mkdir - /usr/local/Frameworks
Error: Permission denied @ dir_s_mkdir - /usr/local/Frameworks

$ brew doctor

