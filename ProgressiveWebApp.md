# Progressive Web App
 
Finally, Hybrid apps will soon be out as most companies are moving towards Native apps using similar tech like React Native. These are Progressive Web Apps (PWA).

PWAs leverage sophisticated web capabilities to deliver in-app experiences to mobile website visitors. 
This includes the ability for visitors to add the website to their mobile home screen, access content while offline, receive mobile notifications from publishers, and more!

It is another term for a website that has been optimized for mobile performance and that utilizes newly available Web APIs to deliver features that are similar to a traditional native app, such as push notifications and offline storage.


PWAs deliver users faster and more dynamic experiences than regular mobile pages.


You can deploy your app as a PWA as well as Native app and take advantage of both channels. Ionic allows you to ship your app to not only the app store, but also deploy to the mobile web as a PWA.

With PWAs, one can offer all the features of an app on their mobile website without changing their CMS, content, or code.


PWA also leverages machine learning to discover important information about visitor browsing habits. It can then adjusts things like menu style and layout to help extend sessions and improve revenue.

## Adding Progressive Web App Support to your app

Adding PWA support to any existing frontend project is easy. Just add an App Manifest file and configure a service worker:

### App Manifest

First, you'll need an App Manifest file (manifest.json) that sits alongside your index.html file and provides metadata about your app, such as its name, theme colors, and icons. This information will be used when your app is installed on the home screen, for example.

### Service Worker

Next, in order to send push notifications and store data offline, a Service Worker will enable your web app to proxy network requests and perform background tasks needed to process and sync data.

Service Workers are powerful, but complicated. Generally, writing them from scratch is not recommended. Instead, take a look at tools like Workbox that provide common Service Worker recipes that you can easily incorporate into your app.


## Progressive Web App Performance

Progressive Web Apps are judged by several performance standards, including Time to Interactive and First Meaningful Paint.

```Time to Interactive - This audit identifies the time at which a page appears to be ready enough that a user can interact with it.```


```First Meaningful Paint - First Meaningful Paint is essentially the paint after which the biggest above-the-fold layout change has happened, and web fonts have loaded.```



### Tools

#### Capacitor: Native Progressive Web Apps

Capacitor is a cross-platform app runtime that makes it easy to build web apps that run natively on iOS, Android, Electron, and the web. We call these apps "Native Progressive Web Apps" and they represent the next evolution beyond Hybrid apps.

Capacitor provides a consistent, web-focused set of APIs that enable an app to stay as close to web-standards as possible, while accessing rich native device features on platforms that support them. Adding native functionality is easy with a simple Plugin API for Swift on iOS, Java on Android, and JavaScript for the web.

Capacitor is a spiritual successor to Apache Cordova and Adobe PhoneGap, with inspiration from other popular cross-platform tools like React Native and Turbolinks, but focused entirely on enabling modern web apps to run on all major platforms with ease. Capacitor has backwards-compatible support for many existing Cordova plugins.



Use Lighthouse to audit and test your app.

If you're struggling to meet Progressive Web App performance standards with your existing frontend stack, take a look at Ionic Framework version 4 (in beta at the time of this writing) or greater as an option for getting fast PWA support with nearly zero configuration. Ionic 4.x or above is a web component library that works in several popular frontend frameworks, not just Angular.

#### Running Natively and on the Web

One of the key features of Capacitor is the ability to build one app that runs both natively (in the app stores), and on the web. Capacitor does this by providing a layer between the underlying platform and the APIs/Plugins you'd like to use.

If your app makes native plugin calls that don't have a web substitute, such as SplashScreen.show(), the app will allow those calls without crashing. Calls that return a promise will return a rejected promise, which you should be handling in your app anyways.

Additionally, Capacitor's JavaScript API has a number of utilities that make it possible to programmatically check whether certain APIs are available.

For example, if your app would normally rely on the Camera app being used to take a photo, you could check if the Camera is available, and if not, ask the user to upload a file instead:

```
import { Capacitor } from '@capacitor/core';

const isAvailable = Capacitor.isPluginAvailable('Camera');

if (!isAvailable) {
  // Have the user upload a file instead
} else {
  // Otherwise, make the call:
  Camera.getPhoto()
}


```

## Hybrid vs Native


### How to make a choice

Most companies face a common challenge, such as, what should be built – native app or hybrid app? Which will be the best for the organization? The answers to the queries depend on the factors such as the following:

1. Speedy development of the app

2. Whether the organization opt for in-house development

3. Objective of building the app

4. Budget to develop the app

5. Features required in the app


### Hybrid

Hybrid applications are web applications (or web pages) in the native browser, such as UIWebView in iOS and WebView in Android (not Safari or Chrome).

Hybrid apps are developed using HTML, CSS and Javascript, and then wrapped in a native application using platforms. like Cordova.



#### The main features of a typical hybrid app are:

1. Faster app development

2. Simple and easy to maintain

3. Cross platform UI

4. Integrate with device file system

5. Less expensive app development and cost effective maintenance

6. Single code management for multiple mobile platforms


### What is Native app?

A native app is a program that has been coded in a specific programming language, for devices having specific OS. For instance, Objective C is used for iOS or Java for Android Phones. These apps can take advantage of OS features and other software tools that are installed on that platform. They also have access to various phones functions such as camera, gallery, contact list etc. Mostly Native apps are compiled into machine code. These provisions help native apps perform the best in a mobile device.

The native development is easy and there are innumerous resources available, but it might not be understandable to everyone. Since the code has to be written specifically for each platform, it has to be rewritten for each one. Only the logic remains same but the language, APIs and the development process might be different. Sometimes, this process becomes quite long for complex applications.


#### The main features of a native app are:

1. High degree of reliability

2. Simple but Fast Performance and better user experience

3. Supports both online & offline transactions

4. Native features can best be exploited


### Development Cost and Time

Hybrid apps take least amount of time to develop and are developed at a fairly cheaper price as compared to native app. Building a hybrid app means maintaining just one code whereas with native code you need an app developer for each platform. But this does not mean that native apps are bad because they have their own advantages.


### User Experience

Native apps provide the best user experience because they are specifically designed for a single app store, with which one can get the best compatible apps. The screen size is taken care of and so the hardware capabilities. With Hybrid apps it is impossible to provide a good experience with just 1 application code for all platforms.


### Paid or Free app

Since native apps have the best UI hence paid apps are usually advised to be developed as native apps whereas free apps can be developed as hybrid apps.