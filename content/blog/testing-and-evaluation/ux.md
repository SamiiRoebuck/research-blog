---
title: 'User Testing'
date: 2020-3-28 16:21:13
category: 'testing and evaluation'
---

**\*User profile**: M, 22, Moved to Leeds recently, using iPhone XS\*

**\*Current state off Kerbit**: almost all required functionality is done\*

---

**General User Comments**

1.  Any way to turn off the red oval around the time?
2.  Double tap zooms on all pages, can this be disabled?
3.  I’d expect pressing the Kerbit logo at the top would take you to the home screen
4.  What can the App actually recognise? Would like to know what things Kerbit actually knows so don't waste time on other things

_Changes/Actions:_

1. Unfortunately this is an inbuilt iOS feature that is used to let the user know when the camera is being accessed by a browser so cannot be changed
2. This will have to be investigated as to whether it can be stopped
3. Noted, the Kerbit logo will return to the initial screen where a new photo can be taken
4. Information of what Kerbit can do could be added in with the how to section so users have a better idea of what Kerbit can be used for

   ***

### Specific app views

**First page, when camera access has been granted**

_User responses:_

1. Flash button does nothing
2. Hide button is confusing as it show the help section, and doesn't hide the popup
3. Can’t tap the view port to focus like you can on camera app, is this possible?

_Changes/Actions:_

1. Flash button implementation to be added
2. Change the icon on the left of the control bar so it is more clear what it will show, maybe to a ?
3. Will have to look into whether this functionality is possible

**When a photo has been taken**

_User responses:_

1. The hide menu button not working when a photo has been taken?
2. On the share page, is there anyway to share the image taken rather than just a generic link?

_Changes/Actions:_

1.  These buttons are disabled at this point, opacity is reduced to indicate this. Will need a more obvious way of showing the buttons are disabled, maybe further reduce the opacity or change the color.
2.  Will have to look into whether the **`navigator.share()`** api allows this, but I do agree that this would be a better use of the share function

**Did Kermit get it wrong screen?**

_User responses:_

1. There’s no way back out of this screen
2. Can scroll on this page and white space appears above and below the app screen, looks weird,

_Changes/Actions_

1.  When making this I assumed that the people going to this screen would be there to submit the form that Kerbit got something wrong, once submitted that gives the way off this screen. Will have to implement a cancel button or something similar for users who unintentionally ended up at this point or have changed their mind and don't want to submit.
2.  Will have to investigate this and see what can stop it, will likely just have to disable any overflow scrolling.

---

These changes and actions will be implemented in the coming days and another post will be written to outline all the changed made.
