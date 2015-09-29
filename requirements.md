# Requirments

In order to create applications with Kandy PhoneGap, you will need to first install the standard SDK for the mobile platforms you want to target for your app. This is because Kandy PhoneGap will actually use these SDKs when compiling your app for that platform.

So, if you are developing for Android, you will need:

There are also some additional PhoenGap specific requirements for Android development, including:

- Eclipse IDE
- ADT plugin for Eclipse
- Apache Ant
- Ruby
- Git Bash (Windows Only)

The PhoneGap Android [documentation] provides the complete list of requirements with install instructions for each.

#### Configure your Android project with Kandy
Add the Kandy SDKs into your Android PhoneGap project and configure project file

- Add Permissions
- Add Services

For more information see [Kandy Android SDK docs].

If you are developing for the [iPhone], you will need:

An intel-based Apple Computer
- iPhone SDK
- Xcode
- Mac OS X Snow Leopard

#### Configure your xcode project with Kandy

Add the Kandy SDKs into your iOS PhoneGap project and configure project file

##### Add the SDK to your app
In order to use the SDK, add the following frameworks to your project:
- KandySDK.framework
- MobileSDK.framework

You can do so by either dragging them to the Project Navigator, or by choosing “Add files” from the Project Navigator Context Menu. For more information see [Kandy iOS SDK docs].


[ documentation]: <http://phonegap.pbworks.com/Getting-started-with-Android-PhoneGap-in-Eclipse>
[iphone]: <http://go.redirectingat.com/?id=1342X589339&xs=2&url=http%3A%2F%2Fwww.amazon.com%2Fs%2Ffield-keywords%3Diphone&xguid=e70bb5849d650d0dc9dbdf495d39860b&xuuid=32d0ce13cc24c8296fc7a893bfeaa0ec&xsessid=7917ca702840f6804ee85fe8fd1fb8ce&isjs=1&xword=iphone&xcreo=300003&xpid=1964102&xed=0&sref=http%3A%2F%2Fcode.tutsplus.com%2Ftutorials%2Fintroduction-to-phonegap-development--mobile-2470&xtz=300>
[Kandy iOS SDK docs]: <https://developer.kandy.io/docs/ios-sdk/>
[Kandy Android SDK docs]: <https://developer.kandy.io/docs/android-sdk/>