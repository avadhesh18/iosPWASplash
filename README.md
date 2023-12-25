ios-pwa-splash
==============

Generate iOS Progressive Web App (PWA) splash screens with ease. Save yourself the hassle of writing multiple meta tags for Apple iPhone and iPad devices. Just provide one icon.png file and a background color.

 [![NPM Version](https://img.shields.io/npm/v/ios-pwa-splash.svg)](https://www.npmjs.com/package/ios-pwa-splash) [![](https://data.jsdelivr.com/v1/package/npm/ios-pwa-splash/badge)](https://www.jsdelivr.com/package/npm/ios-pwa-splash)

Installation
------------

Using jsdelivr CDN

    <script src="https://cdn.jsdelivr.net/npm/ios-pwa-splash@1.0.0/cdn.min.js"></script>
    <script>iosPWASplash('icon.png', '#000000');</script>

Using UNPKG CDN

    <script src="https://unpkg.com/ios-pwa-splash@1.0.0/cdn.min.js"></script>
    <script>iosPWASplash('icon.png', '#000000');</script>    

You can also install `ios-pwa-splash` using npm or yarn:

    npm install ios-pwa-splash
    # or
    yarn add ios-pwa-splash
    

Usage
-----
    
    //Not required if you use CDN
    const iosPWASplash = require('ios-pwa-splash');
    
    // Generate iOS PWA splash screens
    iosPWASplash('path/to/icon.png', 'background-color');
    

*   `icon`: URL or local path to the app icon image (recommended size: 512px x 512px, will be resized based on device pixel ratio).
*   `background-color`: Background color for the splash screen (optional, defaults to 'white').

The `iosPWASplash` function generates iOS PWA splash screens for both portrait and landscape orientations and automatically adds them to the HTML `head` element.

Example
-------
    //Not required if you use CDN
    const iosPWASplash = require('ios-pwa-splash');
    
    // Generate iOS PWA splash screens with a custom background color
    iosPWASplash('path/to/icon.png', '#3498db');
    

Test PWA
-------
Visit https://avadhesh18.github.io/iosPWASplashtest/ from your Apple iPhone or iPad device to test.

Error Handling
--------------

*   If the provided icon URL is invalid or empty, an error will be thrown.
*   If there's an issue loading the icon image, an error will be thrown.

License
-------

This project is licensed under the MIT License.
