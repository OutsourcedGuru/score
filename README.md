# Score
Two-person PhoneGap app for scoring, say, a Scrabble game from your smart phone

I built this application so that my girlfriend and I could score our Scrabble games without relying upon her to... :cough: *occasionally* do the math.

![Score screenshot](https://cloud.githubusercontent.com/assets/15971213/11693078/b1755cd6-9e57-11e5-8760-a5bf070480c2.png)

### Example Code

You can use this as a quickstart to PhoneGap programming.  It includes the necessary style and JavaScript libraries and a minimalized configuration for the least amount of permissions so that your users will trust it.  Clone this code and then create your own cross-platform phone app.

### PhoneGap

[PhoneGap](http://docs.phonegap.com/getting-started/1-install-phonegap/desktop/) is an open source framework for quickly building cross-platform mobile apps using HTML5, Javascript and CSS.  You won't need to learn Objective-C, .Net or Java to write your phone app.

### Testing in Development

I've found that the [PhoneGap Developer App](http://app.phonegap.com) is great for iterative testing of apps before actually building them for production.  You load the **Desktop App** program on your development workstation and point to your folder to serve up the application.  You then complete the pairing by downloading and running the **PhoneGap Developer App** as the client for your phone.  You run this app and point it to the URL that's being served up.

The Desktop App will detect changes to your code as you work on it, recompile and push these changes to your phone within seconds.

It is not necessary to create or upload any certificates or keys in order to test in this fashion so you can get your prototype up and running quickly. 

### Build

It's easiest to build your application for each platform by signing up with [Adobe PhoneGap's Build site](https://build.phonegap.com/plans) using their **Free Plan** to get started.  If you already have an Adobe Creative Cloud membership then you get more than one private app, for example.

Once you've signed up you create a new app profile.  You may then either identify your github site (easiest method) or you may upload a zip file which contains:

1. www\css\\* (as \css\\* in the root folder of the zip file)
3. www\js\\* (as \js\\* in the root folder of the zip file)
4. www\icon.png (as \icon.png in the root folder of the zip file)
7. www\index.html (as \index.html in the root folder of the zip file)
8. config.xml

Follow their directions for creating, uploading and then unlocking each security key per platform as required.  Your certificate then is used to build each platform's application, uniquely identifying yourself as the developer.  After completing this step you build each platform online.  As a developer you may then scan in the QR barcode to download your compiled application for your smartphone.

If you enable their **Hydration** option each time a user starts your application it will check for newer releases and prompt them to install as required.

The alternative to Adobe's build site is to setup multiple build environments on your development workstation, one for each platform.  I've found this to be more trouble than it's worth, tbh.

### JQuery Mobile

Score uses the [jQuery Mobile](http://demos.jquerymobile.com/1.4.5/) framework to render a consistent set of buttons and page navigation throughout.  I highly recommend this platform for all your mobile applications.  Check out their documentation if you are unfamiliar with their syntax.

### Cordova.js

The www/index.html page refers to a JavaScript file cordova.js which does not exist in the source.  This is to be expected and PhoneGap (or your local build environment) creates this file dynamically.

### Phone Platforms

The initial version of Score includes PhoneGap support for the following platforms: Android, iOS.  You can easily add other platforms--assuming that you've correctly installed PhoneGap--using its CLI syntax:

    phonegap run winphone
    phonegap run amazon-fireos
    phonegap run blackberry10
    phonegap run browser
    phonegap run firefoxos
    phonegap run webos

### Notes

* The app currently assumes a Landscape orientation and is best started in this mode.
* There currently isn't a way of reversing an addition if you make a mistake and then press Add.  You can, though, simply remember the two Player's scores, reset the game and then re-enter what they're supposed to be and continue play.

|Donate||Cryptocurrency|
|:-----:|---|:--------:|
| ![eth-receive](https://user-images.githubusercontent.com/15971213/40564950-932d4d10-601f-11e8-90f0-459f8b32f01c.png) || ![btc-receive](https://user-images.githubusercontent.com/15971213/40564971-a2826002-601f-11e8-8d5e-eeb35ab53300.png) |
|Ethereum||Bitcoin|
