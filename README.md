# SwiftUILab

## Setup

```sh
brew install mint
mint bootstrap
```

## XcodeGen

```sh
mint run xcodegen generate
```

## xcodebuild

```sh
xcodebuild -showdestinations -scheme SwiftUILab
xcodebuild -target SwiftUILab build
xcodebuild clean
```

## xcrun

```sh
xcrun simctl install booted ./build/Debug-iphoneos/SwiftUILab.app
xcrun simctl launch booted com.masahikokobayashi.SwiftUILab
```
