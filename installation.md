### Installation

Follow the [wiki] to get started. It includes instructions for using this plugin with iOS and Android devices.

##### Getting Started
This plugin defines a global `Kandy` object, which provide an easy way to interact with Kandy services.
Although the object is in the global scope, it is not available until after the `deviceready` event. After the `deviceready` event, you must initialize configuration and register listeners to use Kandy plugin.

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

See [API Reference](https://github.com/Kandy-IO/kandy-phonegap/blob/master/README.md) for more details.

**Note: To use Kandy plugin, you have to setup `apiKey` and `secretKey` via `initialize` or `setKey` function**

##### How to use example codes

**Create the App**

Go to the directory where you maintain your source code, and  execute the following:

```shell
    phonegap create hello com.example.hello HelloWorld
```

Then, copy example source code from [`demo`] directory of this plugin to your app directory

**Add Platforms**

All subsequent commands need to be run within the project's directory, or any subdirectories within its scope:


```shell
    cd hello
```

Before you can build the project, you need to specify a set of target platforms. PhoneGap Kandy plugin supports both iOS and Android, so run any of these from Mac or Windows machine:

For Android, execute the following:

```shell
    phonegap platform add android
```

For iOS, execute the following:

```shell
    phonegap platform add ios
```

**Add Kandy PhoneGap Plugin**

The `PhoneGap plugin add` command requires you to specify the repository for the plugin code. Here are examples of how you might use the CLI to add features to the app:

For iOS, you need to download and add [Kandy iOS SDK] into 'directory/to/kandy-phonegap/libs/ios/' folder, before adding the plugin into you app and  execute the following,

```shell
    phonegap plugin add directory/to/kandy-phonegap/plugin
```

**Build the App**

For Android, execute the following:


```shell
    phonegap build android
```

For iOS, execute the following:

```shell
    phonegap build iOS
```

[wiki]: <https://github.com/Kandy-IO/kandy-phonegap/wiki>
[Kandy iOS SDK]: <https://developer.kandy.io/docs/ios-sdk/>
[`demo`]: <https://github.com/Kandy-IO/kandy-phonegap/tree/master/demo/www>
