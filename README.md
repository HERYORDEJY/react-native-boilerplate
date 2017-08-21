# React Native Boilerplate

A lightweight react native boilerplate to get you up an running in no time.

Brought to you by Prototype @wizards.

## What's needed

* [Node.js](http://nodejs.org)
* [React](https://github.com/facebook/react) & [React Native](https://github.com/facebook/react-native)

## What's included

* [PropTypes](https://facebook.github.io/react/docs/typechecking-with-proptypes.html)
* [Redux](https://github.com/reactjs/redux) with [redux-thunk](https://github.com/gaearon/redux-thunk) and [redux-persist](https://github.com/rt2zz/redux-persist)
* [React native router flux](https://github.com/aksonov/react-native-router-flux)
* [Immutability helper](https://github.com/kolodny/immutability-helper)
* [React native SVG](https://github.com/react-native-community/react-native-svg)

## Start

* Install node, watchman, and react-native-cli by following this [guide](https://facebook.github.io/react-native/docs/getting-started.html)
* Install Cocaopods:
```
$ sudo gem install cocoapods -n /usr/local/bin
```
* Run the following:
```
$ npm i
$ react-native link
```

#### How to start your own project

* Delete both `ios` and `android` folder. At this stage, those contains nothing that is not autogenerated.
* Change your app name in `app.json`, `package.json`, and `app/index.js`
* Run `react-native upgrade`. This will generate the native folders again.

## Develop

##### iOS

Run command to open iOS simulator and run app:

```
$ npm run ios
```

Or open `ios/RNBoilerplate.xcodeproj` file with XCode:

```
$ npm run ios-open
```

##### Android (5.0+)

Open Android emulator and run:

```
$ npm run android
```


## Test
Test suit is using jest, to run the tests use:

```
$ npm test
```


## Release

#### Build for android

Signing key and password are available on the TW project.

Run `npm run build:android`, Open `/android` in Android studio and follow the process of generating .apk


#### Build for iOS

Certificates and provisioning profiles for dev and prod are available on the TW project.

Open `/ios/.xcodeworkspace`, configure the certificates and follow the normal process of Releasing the app either for app store or for development deployment.
