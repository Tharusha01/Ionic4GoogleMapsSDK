# Ionic4GoogleMapsSDK
Google Maps SDK Cordova Plugin in Ionic 4 Application


Install Ionic Native Google Maps Cordova and Ionic Native Plugin

$ npm install @ionic-native/core@beta @ionic-native/google-maps@beta

$ ionic cordova plugin add cordova-plugin-googlemaps --variable API_KEY_FOR_ANDROID="YOUR_API_KEY_HERE" --variable API_KEY_FOR_IOS="YOUR_API_KEY_HERE"

In the app.component.ts file
initializeApp() {
    this.platform.ready().then(() => {
 
      Environment.setEnv({
        // api key for server
        'API_KEY_FOR_BROWSER_RELEASE': 'YOUR_API_KEY_HERE',
 
        // api key for local development
        'API_KEY_FOR_BROWSER_DEBUG': 'YOUR_API_KEY_HERE'
      });
 
      this.statusBar.styleDefault();
      this.splashScreen.hide();
    });
  }


running command >>>
$ ionic cordova run browser
