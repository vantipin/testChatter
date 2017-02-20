# Wordfinder

![Wordfinder](https://cloud.githubusercontent.com/assets/16136204/22782513/79078ef0-eed8-11e6-8108-d695bda9765a.jpg)

[![license](https://img.shields.io/github/license/mashape/apistatus.svg)]()
[![Platform](https://img.shields.io/badge/platform-iOS-lightgrey.svg)]()
[![Language](https://img.shields.io/badge/language-swift%203%20%7C%20objc-green.svg)]()

Wordfinder is a reference application created by [Digiteum](http://www.digiteum.com/) to showcase usage of [Oxford Dictionary API](https://developer.oxforddictionaries.com).

- [x] Client-side application
- [x] Restful architecture
- [x] Single view application

## Requirements

- iOS Deployment Target 9.3+
- XCode 8.2+
- Swift 3.0.2

## Try it now

You can download app from  [App Store](https://itunes.apple.com/us/app/wordfinder-your-personal-crossword/id1199800362?ls=1&mt=8)

![Wordfinder](https://cloud.githubusercontent.com/assets/16136204/22782512/79050acc-eed8-11e6-9f40-3d39e8c07390.gif)

## Installation
#### API keys Authentication
To run project you'll need to get your own copy of [Oxford Dictionary API](https://developer.oxforddictionaries.com/documentation/getting_started) keys. 
[Register](https://developer.oxforddictionaries.com/?tag=#plans) an account and go to [API Credentials](https://developer.oxforddictionaries.com/admin/applications) to get app_id and app_key. Alternatively you can find your API keys in [Swagger interface](https://developer.oxforddictionaries.com/documentation) after you login in your account.

Keys need to be placed in `DGTRequestFactory.m`
```objective-c
18| static NSString* APP_ID = @"";
19| static NSString* APP_KEY = @"";
```

## Usage
Find word that match search parameters. 
- Type in first letter.
- Type in any other letter. [optional]
- Change number of letters. [optional]
- Change part of speech. [optional]
- `Search` to make query to Oxford API.
- View/copy results.

## Project comments
- Network. Conversation with API done via Network Manager library. It's a powerful interface designed to control life cycle of multiple instances of NSURLSessionDataTask. You can start exploring it from `DGTNetworkManager`.


## License

Wordfinder uses the MIT license. Please file an issue if you have any questions or if you'd like to share how you're using this project.
