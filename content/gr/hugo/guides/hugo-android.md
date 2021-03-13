---
title: "Hugo Android"
date: 2021-03-06T12:35:06+01:00
draft: "false" # Set to false to publish
author: "Code-XS"
description: "Put your description here" 
summary: "Put your summary here" 
tags: [Guide] 
categories: [Hugo] 
## HERO IMAGE ##
# You have to fill the heroImageUrl and the heroImageDescription.
HeroImage: "false" # Change to true if you want to enable hero images
HeroImageUrl: "HERO IMAGE URL"
HeroImageDescription: "HERO IMAGE DESCRIPTION"
HeroImageWidth: ""
HeroImageHeight: ""
## DROPCAP ##
EnableDropcap: "true" #Set to false to disable dropcap
## DISCLAIMER ##
Disclaimer: "false"
DisclaimerTitle: "Disclaimer"
DisclaimerContent: "This is demo content taken from the original article in Wikipedia. It is depicted hare purely for demonstrative reasons."
## STRUCTURED DATA ##
StructuredDataType: "article"
---

If for some reason you want to run hugo locally on your android device, you can follow the steps.

1. Install [Termux](https://termux.com/ "Termux Website") from [F-droid](https://www.f-droid.org/ "F-droid Website") or ~~Google Play store~~. Since 22 November 2020 Google Play version of the Termux app will no longer
receives updates according to the [Termux Wiki](https://wiki.termux.com/wiki/Termux_Google_Play "Termux Wiki"). It is recommended to install the F-droid version.

1. Open Termux app and run the command
   
``` bash 
apt update && apt upgrade
```
When you are asked if you want to continue write Y and press enter. (If during the update termux asks you if you want to Replace or Keep the current version  press Y to replace or N to use the default option.

1. Install hugo with the command
``` bash
pkg install hugo
```
4. Now run 
``` bash
termux-setup-storage
```
and press allow to the pop-up  to give storage access.
     
5. Create a folder in your internal storage where your site workspace will be located by using the command from termux
``` bash 
create folder command
```
or with your device file manager.

6. From termux run
``` bash
cd /storage/shared/YOUR-FOLDER
```

7. Run 
``` bash
hugo server -D
```

8. All done your local site will be accessible from your browser at the address 
```
http://localhost:1313/
```
### Tips and tricks
* You can see your current working folder with the command 
``` bash
 pwd
```
 * You can see a list of the subfolders of your current folder with the command
``` bash
ls
```

This guide is inspired and based on a comment of the github user [sumit-buddy](https://github.com/sumit-buddy)

---