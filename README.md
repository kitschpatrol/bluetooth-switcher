# bluetooth-switcher

To install:

1. Install blueutil: `brew install blueutil`
2. Save bluetooth-switcher.app to Applications (or anywhere that makes sense).
3. Open bluetooth-switcher.app, you'll probably need to give it some permissions.
4. On your mac, open Preferences > Users & Groups. Select your name, and add bluetooth-switcher to startup apps. 

Next time you log in it will automatically start.

## Rebuilding
Open the bluetooth-switcher.applescript in Apple's Script Editor tool and export it as an application (File > Export). Check the "Stay open after run handler" option.

## Hiding the app from the dock
If you'd prefer the app to not show up in the dock, run the following. (Assumes an installation to the Applications folder.)

`defaults write '/Applications/bluetooth-switcher.app/Contents/Info.plist' LSUIElement -bool yes`
