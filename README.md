# react-native-webview-scrollview-crash
A reproduction code for android app crash on scroll end when using webview nested inside scrollview.
The code is just an extension to default boilerplate code from react-native, only line added nested inside
scroll view is this one...

`<WebView style={{height:200}} source={{html:"<p>This is web body</p>"}} ></WebView>`
https://github.com/noumantahir/react-native-webview-scrollview-crash/blob/f3987c110404d9e964f7b760efa4ed8169bf70d5/App.js#L70

This is enough to cause app to crash on scroll

## build instruction
- gh repo clone noumantahir/react-native-webview-scrollview-crash
- cd react-native-webview-scrollview-crash
- yarn
- npx react-native run-android

## reproduce crash
- scroll down to very bottom
- android app will crash
