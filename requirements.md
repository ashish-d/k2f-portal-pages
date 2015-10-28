### Requirements

In order to create applications with Kandy features, you will need to first install the Kandy native mobile SDKs for the mobile platforms you want to target for your app. The PhoneGap Kandy plugin will actually use these SDKs when compiling your app for that platform.

**if you are developing for Android, you will need:**

- Eclipse IDE
- ADT plugin for Eclipse
- Apache Ant
- Ruby
- Git Bash (Windows Only)

The PhoneGap Android [documentation] provides the complete list of requirements with install instructions for each.

**Configure your Android project with Kandy:**

Add the Kandy SDKs into your Android PhoneGap project and configure project file

- Add Permissions
- Add Services

For more information see [Kandy Android SDK docs].

**If you are developing for the iOS, you will need:**

An intel-based Apple Computer

- iPhone SDK
- Xcode
- Mac OS X Snow Leopard

**General Configuration:**

##### Enable Background Mode

For the application to work as expected in the background, enter into the application's Info.plist the following configuration:

```markup
<key>UIBackgroundModes</key>
<array>
  <string>audio</string>
  <string>voip</string>
</array>
```
For more information see [Kandy iOS SDK docs].


[documentation]: <http://phonegap.pbworks.com/Getting-started-with-Android-PhoneGap-in-Eclipse>
[Kandy iOS SDK docs]: <https://developer.kandy.io/docs/ios-sdk/>
[Kandy Android SDK docs]: <https://developer.kandy.io/docs/android-sdk/>
