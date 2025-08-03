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
xcodebuild -showsdks
xcodebuild -showdestinations -scheme SwiftUILab

# Simulator
xcodebuild clean
xcodebuild -target SwiftUILab -sdk iphonesimulator18.5 -destination 'platform=iOS Simulator,id=4EA2495F-FB61-4C94-AF9E-A83EC03C6233' build

xcodebuild -scheme SwiftUILab -only-testing:SwiftUILabTests -destination 'platform=iOS Simulator,id=4EA2495F-FB61-4C94-AF9E-A83EC03C6233' test
```

## xcrun

```sh
# Simulator
xcrun simctl install booted ./build/Debug-iphonesimulator/SwiftUILab.app
xcrun simctl launch booted com.masahikokobayashi.SwiftUILab
```
