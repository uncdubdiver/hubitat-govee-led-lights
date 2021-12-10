# hubitat-govee-led-lights
Govee LED Light Strips integration for Hubitat Elevation

### Pre-requisites
Must have a Hubitat Elevation Hub
Govee LED Light Strips
Govee API Key (generated from the Govee mobile app)

### To integrate this into Hubitat, you'll follow these steps:
![#f03c15](https://via.placeholder.com/15/f03c15/000000?text=+) To properly integration into Hubitat Elevation, please go to the following URL: https://www.deanberman.com/govee/hubitat/
This page will provide you step-by-step procedures on add the device and device type handlers into your Hubitat account.  You provide it your Govee API Key and it will retrieve the list of device ids, names, and models for the device preferences.

If you are more comfortable running the file(s) locally and have a webservice and php enabled locally, then you may download the index.html and the \_devices.php file and implement them locally (just update the index.html file for the URL reference location).

#### The following list of model numbers are currently supported (according to Govee API document):
- H6160
- H6163
- H6104
- H6109
- H6110
- H6117
- H6159
- H7021
- H7022
- H6086
- H6089
- H6182
- H6085
- H7014
- H5081
- H6188
- H6135
- H6137
- H6141
- H6142
- H6195
- H6196
- H7005
- H6083
- H6002
- H6003
- H6148

### DEBUGGING/TROUBLESHOOTING
If you edit the driver code in your local Hubitat environment, search for the "refresh()" function and enable debugging by setting the following:  
```groovy
set_DEBUG("off")
...to...
set_DEBUG("on")
```

### DRIVER DISCLAIMER
After further testing, the API call for getting the device state may not work for all supported Govee models listed above.  Determing if it's a problem with the Govee API or if it's not supported due to the nature of the device model.

### DISCLOSURE
I am not a Hubitat developer, I just did this because I wanted to be able to integrate my multiple Govee LED Light strips into my Smart home network, so I created this myself.  It works well for me and this isn't for sale, so feel free to use it, tweak it, whatever you want!
Just a heads up, this isn't perfect by any means, so feel free to provide me some input and updates, I'll be happy to make them!

Your support will help further the development and integration of this driver code and other devices which may/may not be supported as of yet with Govee!

Enjoy!
