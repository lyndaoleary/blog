+++
date = "2014-10-28T00:00:00+00:00"
title = "Update Unavailable with This Apple ID"
tags = ["computing"]
+++

So I just got my new Macbook with Mavericks installed, and when updating to Yosemite I came across this issue when attempting to update the iLife and iWork suite.

	Update Unavailable with This Apple ID
	This update is not available for this Apple ID either because
	it was bought by a different user or the item was refunded
	or cancelled.

I went to the website for Apple support, they called back straightaway but then was in the queue for around 5 minutes.  Tried a few things (which I will list below as well), but here's the solution that worked for me.

* Navigate to Applications and move iMovie and iPhoto to the Trash
* Open App Store and search for iMovie, accept and install this.  If you get an error "Update has already been accepted" then click on the purchases tab and click on install for the app
* Repeat the above step for iPhoto
* Re-attempt update of the rest of the iWork/iLife suite, if you get issues with updating other apps then try removing them and re-installing from the App Store as per steps 2 and 3


If that doesn't work, here are a few options that were attempted prior to the solution that worked for me:

* Created a new user called test, signed in with the same Apple ID and tried again, no luck
* Moved /Library/Preferences/com.apple.storageagent.plist to Desktop temporarily and then re-ran update
* Moved to desktop the following files/directories and re-ran update:
  * /Users/myusername/Library/Preferences/com.apple.appstore.plist
  * /Users/myusername/Library/Containers/com.apple.appstore
  * /Users/myusername/Library/Containers/com.apple.appstore.PluginXPCService
* When in App Store, select Store from the menu bar at the top of the screen, and select sign out.  Sign back in and re-attempt the update.
