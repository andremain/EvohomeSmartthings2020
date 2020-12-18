# EvohomeSmartthingsNew
A modified Evohome Smartthings integration based on Codersaur's code from 2016.

Release is now live! - 18/12/2020

Changes from the old app:

Fixed the API endpoint to be the new one that Honeywell Evohome uses
Added The new capababilities for the depricated thermostat capability used by the new smartthings app
Fixed the Checking Status on the dashboard tile for use with the new Smartthings app
Generated the Presentation file required by the new smartthings app for correctly displaying the options for the inside of the new app
Removed the old custom and deprecated capabilities from the old code
Changed the default value for window function temperature from 5.0 to 5 as it would throw a bad request error
Managed to get the correct thermostat modes to show app in the modes list in the new app presentation
Managed to get the modes to work with the new app’s presentation. Some list items appear weird but this is a Smartthings issue
Changed the links for the documentation and images to work.
Removed the cooling options
Known issues:

Cannot set the temperature and an error is thrown.

You need to reinitialize the device handlers. The solution to this is to get the Evohome Connect SmartApp to resend the device id to the device handler. Fortunately you can do this going into the Evohome Connect SmartApp and changing a setting (I changed the polling period) which causes a refresh of the data.



