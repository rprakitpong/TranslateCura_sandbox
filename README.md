# TranslateCura_sandbox
Python script for automating Cura translation for free, using googletrans and polib

# How to get started

## Tools required
*[Latest version of Python](https://www.python.org/downloads/)
* * Add it to PATH
*[polib](https://pypi.org/project/polib/)
* * You need to get Python before this
*[googletrans](https://pypi.org/project/googletrans/)
* * You need to get Python before this
* po file editor of choice
* git bash or Github Desktop
* * If you don't want to use git, you can also get all starter files [here](http://s000.tinyupload.com/index.php?file_id=46164836594148367166) (last updated 2020/04/08)
* VPN
* * I recommend [Windscribe](https://windscribe.com) because it gives you multiple IPs for free
* Optional: any modern IDE (VS Code is pretty good)

## Steps
Download translate.py and [the four files needed to be translated](https://github.com/Ultimaker/Cura/wiki/Translating-Cura):
* Clone this repo to get translate.py and the 4 pot files (they're in cleanStarter)
* Clone Cura and Uranium to get latest version of pot files
* Download [this](http://s000.tinyupload.com/index.php?file_id=46164836594148367166) if you don't want to use git

Make sure the 4 pot files are in the same directory as translate.py.

Open translate.py and edit destLang to your language of choice:
* Notepad will open Python files just fine
* Although having a good IDE helps 
* To get list of available langugages, run this in command prompt:
``` python
import googletrans
googletrans.LANGUAGES
```

Run translate.py:
* Double click on .py file to run
* Run inside your IDE for nicer interface

At some point, it will stop. Use your VPN to change your IP, then run again. Repeat until you burn through all your free connections, then wait a few days to get unblocked. 

Repeat until everything is translated. Check po files periodically to check how far things are translated. You should verify and edit the translations as Google Translate isn't perfect.

Submit your translations by pull request or emailing r.dulek@ultimaker.com. 

# Limitations
* Will blindly translate XML tags (fixing manually is ok for now since there's only 29 of these in all 4 files)
* googletrans wil die sometimes (json.decoder.JSONDecodeError) because Google doesn't like it. Wait a few days or use VPN.

# TODO
comment on code