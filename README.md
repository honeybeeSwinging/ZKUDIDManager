# ZKUDIDManager

[![Travis-CI](https://travis-ci.org/mushank/ZKUDIDManager.svg?branch=master)](https://travis-ci.org/mushank/ZKUDIDManager) [![Carthage](https://img.shields.io/badge/carthage-compatible-green.svg)](https://github.com/Carthage/Carthage) [![CocoaPods](https://img.shields.io/badge/pod-1.0.8-green.svg)](http://cocoapods.org/?q=ZKUDIDManager) [![Platform](https://img.shields.io/badge/platform-iOS-lightgrey.svg)](http://www.apple.com/ios) [![License MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/mushank/ZKUDIDManager/blob/master/LICENSE)


**Generate and save permanent UDID with IDFV and keychain in iOS device.**

*Use `IDFV(identifierForVendor)` + `keychain` to make sure UDID consistency, even if the App has been removed or reinstalled.*

*A replacement for the deprecated mean of `OpenUDID`.*

## Install

#### CocoaPods

Available through [CocoaPods](http://cocoapods.org/), simply add the following line to your Podfile:

```
pod 'ZKUDIDManager', '~> 1.0'
```

#### Carthage

Available through [Carthage](https://github.com/Carthage/Carthage), simply add the following line to your Cartfile:

```
github "mushank/ZKUDIDManager" ~> 1.0
```

*Noti: Requires iOS 6.0 or later*

## Usage
It's so simple, just two lines of code:

```
#include "ZKUDIDManager.h"
NSString *UDIDString = [ZKUDIDManager value];
```

⚠️***Attention:*** *If you get the value `(null)`, please check your `KeyChain Entitlemen` setting: Go to project settings->Capabilities->Keychain Sharing->Add Keychain Groups+Turn On*. It usually happens in iOS 10.

## Source files

They are in the `ZKUDIDManager` folder:   

- `ZKUDIDManager.h`  
- `ZKUDIDManager.m`  

Now, enjoy yourself!

## License

ZKUDIDManager is released under [MIT License](https://github.com/mushank/ZKUDIDManager/blob/master/LICENSE).