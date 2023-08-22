# Hiddify Next

<p align="center"><img src="assets/images/logo.svg" width="168"/></p>

<p align="center" style="font-size: 20px">Hiddify Multi-platform Proxy Client</p>
<p align="center" style="font-size: 20px">⚠️Hiddify Next is still in early development phase⚠️</p>
<p align="center" style="font-size: 16px">Windows, Android, Linux and macOS are supported (PR for iOS welcome)</p>

## Download Hiddify Next Pre-Release 
- Android: [Universal](https://github.com/hiddify/hiddify-next/releases/download/draft/hiddify-android-universal.apk) - [Arm64](https://github.com/hiddify/hiddify-next/releases/download/draft/hiddify-android-arm64.apk) - [Arm7](https://github.com/hiddify/hiddify-next/releases/download/draft/hiddify-android-arm7.apk)  - [x86_64](https://github.com/hiddify/hiddify-next/releases/download/draft/hiddify-android-x86_64.apk)
- Windows: [x64 Setup](https://github.com/hiddify/hiddify-next/releases/download/draft/hiddify-windows-x64-setup.exe) - [x64 Portable](https://github.com/hiddify/hiddify-next/releases/download/draft/hiddify-windows-x64-portable.zip)
- Linux: [x64 AppImage](https://github.com/hiddify/hiddify-next/releases/download/draft/hiddify-linux-x64.AppImage)
- macOS: [Universal (x64, M1, M2)](https://github.com/hiddify/hiddify-next/releases/download/draft/hiddify-macos-universal.dmg)
## Build from source

### requirements:
  - GO v1.21+
  - Flutter v3.10+
  - Make
  - GCC
  - MinGW-w64
  - Android SDK (with CMake and NDK)

  This project uses [flutter_distributor](https://github.com/leanflutter/flutter_distributor) for packaging.

  ```shell
  # fetch dependencies and build generated files
  $ make get gen

  for platform in [windows linux macos android]:
     # build native library
     $ make $platform-libs windows-libs
     $ make release-$platform
  
  # example:
     $ make windows-libs
     $ make windows-release
  ```

## Acknowledgements
  - [Singbox](https://github.com/SagerNet/sing-box)
  - [Clash](https://github.com/Dreamacro/clash)
  - [Clash Meta](https://github.com/MetaCubeX/Clash.Meta)
  - [FClash](https://github.com/Fclash/Fclash)
