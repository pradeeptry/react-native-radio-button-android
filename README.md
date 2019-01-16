# React Native Radio button for Android

Native Android radio-button component, orignally forked from [here](https://github.com/sichacvah/react-native-radio-button-android).

## Installation

```
yarn add react-native-radio-button-android
// or with npm
npm i react-native-radio-button-android --save
```

1. `android/settings.gradle`:: Add the following snippet

```gradle
include ':react-native-radio-button-android'
project(':react-native-radio-button-android').projectDir = new File(rootProject.projectDir, '../node_modules/react-native-radio-button-android/android')
```

2. `android/app/build.gradle`: Add in dependencies block.

```gradle
dependences {
  ...
  compile project(':react-native-radio-button-android')
}
```

3. `android/app/src/main/java/com/<your_app>/MainActivity.java`: Import package and add to react list of packages.

```java
import io.sichacvah.react.radio_button.RadioButtonPackage;
...

protected List<ReactPackage> getPackages() {
  return Arrays.<ReactPackage>asList(
    ...
    new RadioButtonPackage()
  );
}
```

### License: ISC
