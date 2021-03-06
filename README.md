# Locale
Javascript location function that returns a promise chain with a device's current location.

## Preface
Locale is a Javascript micro framework that was designed to handle retrieving the GPS location of your device.  The promise structure is a more accessible method of retrieval than the navigator API.  It is some what a facade class.

## Example
```
var deviceLocation = locale();
deviceLocation.then(function(location){
   console.log("lon: " + location.longitude + ", lat: " location.latitude); 
});
```
Returns the devices location with the default options.

```
var deviceLocation = locale({enableHighAccuracy : false});
deviceLocation.then(function(location){
   console.log("lon: " + location.longitude + ", lat: " location.latitude); 
});
```
Returns the devices location with the non default option enableHighAccuracy = false.

## License
The MIT License