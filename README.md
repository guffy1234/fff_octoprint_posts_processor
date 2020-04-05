Generic FFF Fusion 360 CAM posts processor with OctoPrint support
====

This is modified fork of Autodesk's Generic FFF post processor

![screenshot](/screenshot.jpg "screenshot")

It seems that XMLHttpRequest class exists in the PP objects model, but unfortunatelly it doesn't work properly.
So the post processor uses CURL for uploading.
You can take CURL [here](https://curl.haxx.se/download.html) and have to put binary files to same foleder where post processor file resides.

![screenshot_curl](/screenshot_curl.jpg "screenshot_curl")

Due to existing execute function call in the code of the post processor Fusion 360 (launching curl) 
will warn you with following dialogue.

![screenshot_warn](/screenshot_warn.jpg "screenshot_warn")

You have to press "Yes" button.

# User Properties

## Group 1: Octoprint properties

|Title|Description|Default|
|---|---|---|
Octo: URL|Octoprint URL|
Octo: API|High speed for travel movements X & Y (mm/min).||
Octo: Start print|Start printing immediatelly|**false**|
Curl: Hide|Hide curl application|**false**|
