# SeaCat client bridge for React Native on iOS

The small bridge that enables iOS/React Native developers to use SeaCat.  
Works now for HTTP calls (e.g. fetch()). Websocket support is not implemented yet.

More about SeaCat at [TeskaLabs.com](http://teskalabs.com/).

# Example of use

It basically allows you to made SeaCat calls directly from React Native JS environment:

```javascript
  	fetch('https://host.seacat/endpoint')
  		.then((response) => response.text())
		.then((responseText) => {
			console.log(responseText);
	});
```

# Implementation

First, integrate SeaCat SDK with React Native iOS app in a normal way.
It is explained e.g. here: http://www.teskalabs.com/blog/trial_for_ios_mac_osx (seek for 'Installation of SeaCat client' chapter).

Then, simply drag-n-drop SeaCatReactNativeBridge folder into your iOS app project in XCode.

![alt tag](https://raw.githubusercontent.com/TeskaLabs/SeaCat-ReactNative-iOS/master/docs/step01.png)

![alt tag](https://raw.githubusercontent.com/TeskaLabs/SeaCat-ReactNative-iOS/master/docs/step02.png)

![alt tag](https://raw.githubusercontent.com/TeskaLabs/SeaCat-ReactNative-iOS/master/docs/step03.png)
