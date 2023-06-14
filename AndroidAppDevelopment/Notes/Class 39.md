[Location](https://developer.android.com/training/location/retrieve-current)

1. What are the benefits and downfalls of using the ‘getLastLocation()’ method to get your device’s location?
	1. the downfalls are that it could return null due to these reasons 
		1. - Location is turned off in the device settings. The result could be `null` even if the last location was previously retrieved because disabling location also clears the cache.
		   - The device never recorded its location, which could be the case of a new device or a device that has been restored to factory settings.
		   - Google Play services on the device has restarted, and there is no active Fused Location Provider client that has requested location after the services restarted. To avoid this situation you can create a new client and request location updates yourself. For more information, see [Receiving Location Updates](https://developer.android.com/training/location/receive-location-updates).
	2. the upsides are 
		1. - [`getLastLocation()`](https://developers.google.com/android/reference/com/google/android/gms/location/FusedLocationProviderClient#getLastLocation()) gets a location estimate more quickly and minimizes battery usage that can be attributed to your app. DOWNSIDE --- However, the location information might be out of date, if no other clients have actively used location recently.
1. What about the ‘getCurrentLocation()’ method?
	1. [`getCurrentLocation()`](https://developers.google.com/android/reference/com/google/android/gms/location/FusedLocationProviderClient#getCurrentLocation(int,%20com.google.android.gms.tasks.CancellationToken)) gets a fresher, more accurate location more consistently. However, this method can cause active location computation to occur on the device