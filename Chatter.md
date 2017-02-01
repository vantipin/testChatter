# Chatter
[![license](https://img.shields.io/github/license/mashape/apistatus.svg)]()
[![Platform](https://img.shields.io/badge/platform-iOS-lightgrey.svg)]()
[![Language](https://img.shields.io/badge/language-objc-green.svg)]()

Chatter is a reference application created to showcase [Oxford Dictionary API usage](https://developer.oxforddictionaries.com).

- [x] Client-side application
- [x] Restful architecture
- [x] Chatbot

## Requirements

- iOS Deployment Target 9.3+
- Xcode 8.2+
- CocoaPods 1.2.0+

## Try it now
You can download app from [Appstore](https://itunes.apple.com/us/app/chatter-learn-language-oxford/id1199793820?ls=1&mt=8)

## Installation

#### CocoaPods
[CocoaPods](http://cocoapods.org) is a dependency manager for Cocoa projects. You can install it with the following command:

```bash
$ gem install cocoapods
```

Pull repository. Change directory to `/Chatter`. You'll need to run 
```bash
$ cd ./Chatter
$ pod update
```
Pods will generate `Chatter.xcworkspace`. Run it with xcode.


#### API keys Authentication
To run project you'll need to get your own copy of [Oxford Dictionary API](https://developer.oxforddictionaries.com/documentation/getting_started) keys. 
[Register](https://developer.oxforddictionaries.com/?tag=#plans) an account and go to [API Credentials](https://developer.oxforddictionaries.com/admin/applications) to get app_id and app_key. Alternatively you can find your API keys in [Swagger interface](https://developer.oxforddictionaries.com/documentation) after you login in your account.

Keys need to be placed in `DGTCoreNetworkConstants.h`
```objective-c
36| 
37| #define APP_ID @""
38| #define APP_KEY @""
```

## Usage
- Game "Guess a word". Choose category by tapping corresponding button. Read the definition and try to guess the word. Type the answer. 
- Switch mode.
- Translation. Choose language. Type the word.

## Project structure
- Actions. Chatbot behaviour controlled via Actions.
- Categories. Extensions of standard classes.
- Network. Conversation with API done via Network Manager library. It's a powerful interface designed to control life cycle of multiple instances of NSURLSessionDataTask. You can start exploring it from `DGTNetworkManager`.


## License

Chatter uses the MIT license. Please file an issue if you have any questions or if you'd like to share how you're using this project.
