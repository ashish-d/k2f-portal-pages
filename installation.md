## Installation
Check out PhoneGap CLI [docs](http://docs.phonegap.com/en/3.0.0/guide_cli_index.md.html#The%20Command-line%20Interface)
before starting out.

    cordova plugin add "path/to/kandy-phonegap/directory"
or

    cordova plugin add https://github.com/kodeplusdev/kandyphonegap.git
## Getting Started
This plugin defines a global `Kandy` object, which provide an easy way to interact with KANDY.
Although the object is in the global scope, it is not available until after the `deviceready` event. After the `deviceready` event, you must initialize to  config and register listeners to use Kandy plugin.

```js
    function onDeviceReady(){
        ...
        Kandy.initialize({
            apiKey: "api",
            secretKey: "secret"
        });
    }
```
After you initialize the `KandyPlugin`, you can use `Kandy` with following syntax:
```js
    Kandy.access.login(function(s){ // successCallback function
        // your code here
    }, function(e){ // errorCallback function
        // your code here
    }, username, password);
```
or as a widget:
```html
    <kandy widget="call" call-success="callSuccess"></kandy>
```
See [API Reference](#api-reference) for more details.

**Note: To use Kandy plugin, you have to setup `apiKey` and `secretKey` via `initialize` or `setKey` function**

## How to use example codes
**Create the App**

Go to the directory where you maintain your source code, and run a command such as the following:
```shell
    phonegap create hello com.example.hello HelloWorld
```
Then, copy example source codes from [`demo`](/demo) directory of this plugin to your app directory

**Add android platform**

Run a command such as the following:
```shell
    phonegap platform add android
```
**Add iOS platform**

Run a command such as the following:
```shell
    phonegap platform add ios
```
**Add plugin**

Go to your app directory and run a command such as the following:
```shell
    phonegap plugin add directory/to/kandy-phonegap/plugin
```
**Build the App Android**

Run a command such as the following:
```shell
    phonegap build android
```
**Build the App iOS**

Run a command such as the following:
```shell
    phonegap build iOS
```