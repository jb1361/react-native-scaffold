# react-native-scaffold
A scffolded project for creating react-native apps

# Build
```cd app && npm i```

## IOS react-native-config
* Go to your project -> Build Settings -> All
* Search for "preprocess"
* Set Preprocess Info.plist File to Yes
* Set Info.plist Preprocessor Prefix File to ${BUILD_DIR}/GeneratedInfoPlistDotEnv.h
* Set Info.plist Other Preprocessor Flags to -traditional
* If you don't see those settings, verify that "All" is selected at the top (instead of "Basic")

## Optional dependencies
* Bugsnag is currently installed to have remote error reporting.
Uninstall:
* react-native unlink bugsnag-react-native
* npm uninstall bugsnag-react-native
* remove from index.js
```import { Client } from 'bugsnag-react-native';
const bugsnag = new Client("3d3f6ed00f43fa9815379c72e47384c4");
```


