# How to Package MacOS

At this time you can not build the MacOS app via the PWA Builder Web Site, so you'll need to build this app via the CLI tool.  MacOS is supported in the [macOS platform module](https://www.npmjs.com/package/pwabuilder-mac) for pwabuilder.

1. Make sure **pwabuilder** installed. If not, install using: 

`npm install -g pwabuilder`

2. Add **macOS platform** by:

 'pwabuilder platform add mac pwabuilder-mac'

3. Then, use pwabuilder to generate the polyfills: 

'pwabuilder https://btdj.azurewebsites.net/ -d C:\Projects -l debug -p mac'

  Parameter |  Description
 --- | --- 
 *-d* | the directory you would like to generate the app
 *-l* | the log level of the CLI
 *-p* | the platforms to build


 

**Note** if you would like to submit the app to the mac store, continue on with step 4 and 5


4. You'll need to download and install [Xcode](https://developer.apple.com/xcode/downloads/)

5. Then, you can follow the[ Submitting Your App to the Store](https://developer.apple.com/library/content/documentation/IDEs/Conceptual/AppDistributionGuide/SubmittingYourApp/SubmittingYourApp.html) steps in the Apple's App Distribution Guide.
