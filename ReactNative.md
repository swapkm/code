## Released APK

`cd android && ./gradlew assembleRelease`
`cd android && ./gradlew bundleRelease`
`adb install -r android/app/build/outputs/apk/release/app-release.apk`
```
    cd ..
    rm -rf android/app/src/main/res/drawable-*
    react-native bundle --platform android --dev false \
      --entry-file index.js \
      --bundle-output android/app/src/main/assets/index.android.bundle \
      --assets-dest android/app/build/intermediates/res/merged/release/
    cd android && ./gradlew assembleRelease
```
`cd android && ./gradlew clean`
`rm -rf android/app/src/main/res/drawable-*`
