---
cover:
 image: /images/ghazigram.png
 alt:
 relative: false
title: 'Ghazigram Setup in Termux & Terminal Guide'
author: 'inishaikhalishan'
date: 2025-03-10T21:55:19+05:30
tags:
  - 
draft: false
categories:
  - Ghazigram
  - bot setup
  - guid
--- Ghazigram is a multiFutered Telegram userbot.

If you want to Setup Ghazigram, so you have to follow few steps.

# Setup Termux
If you want to Setup Ghazigram in Termux on your android device Then follow these steps.

**Install Termux**: First of all you must have Termux installed on your Android device.

If you don't have it then you can simply install it from Google Playstore.

[Termux Link Google Playstore](https://play.google.com/store/apps/details?id=com.termux)

**Storage setup in Termux**: After installing Termux.

First you'll need to grant Termux access to your device's storage.

Run this command in Termux:
```shell
termux-setup-storage
```

This command will request permisson to access your device's storage.

# Setup Ghazigram Termux/Terminal

**Update**: Before installing Python , It's good idea to update the Termux packages list and upgrade the installed packages:

First run this command:
```shell
pkg update
```

And then run this:
```shell
pkg upgrade 
```


**Install Python:** Once the package list is updated, install Python.

By running this command:
```shell
pkg install python
```


**Install Git:** We need a git package to clone the repository.

Run this command and install:
```shell
pkg install git 
```

**Clone Repository**: packages installation is done, Now we need to clone the repository.

By running this commaand: 
```shell
git clone https://github.com/inishaikhalishan/Ghazigram.git
```

**Install Ghazigram Requirements**: After cloned the repository, Then check it.


Run this:
```shell
ls
```


then you see You have a `Ghazigram` named directory, Now we need to go in repository.


Run this command:
```shell
cd Ghazigram 
```

Now we will install the requirements.

Simply run this:
```shell
pip install -r requirements.txt
```

# Generate Telegram Account Session
First we need to Telegram App API_ID & API_HASH.

if you don't have then you generate from Telegram Official Website [my.telegram.org](https://my.telegram.org)

After generating then Generate the string session from Ghazigram repository.

Go to Terminal/Termux and go to in Ghazigram directory.

And then run this command:
```shell
python string_session.py
```

Just copy and paste api_id & hash and then copy string_session  from your client save message.


# Sign in Ghazigram
Before sign in, We need to create .env file.

.env file is used to keep your private things so that no one can access it.

create .env file and open it By run this command:
```shell
nano .env
``` 


After open .env file then paste this contant in .env file.
```shell 
api_id=YOUR_API_ID
api_hash=YOUR_API_HASH
string_session=YOUR_STRING_SESSION
```

Reaplace `YOUR_API_ID`, `YOUR_API_HASH`  and `YOUR_STRING_SESSION` with yours.

Then Click `Ctrl+s` and Then `Ctrl+x`

# Run Ghazigram 
Now all are good, Run the Ghazigram.

Go to root Directory:
```shell
cd Ghazigram
```

Now run the Ghazigram:
```shell
python -m ghazigram 
```

And Ghazigram Successfully Started.

You can check By Running this command in Telegram chat:
```shell
/tts Hello, Ghazigram
```



**Shortcut to run the Ghazigram to Home directory by .sh file:** If you want to run ghazigram to home directory by one command then you need to create the .sh file, Follow few more steps.


first you go to home directory by the command:
```shell 
cd ..
```

Then create ghazigram_run.sh file, You can add any name.

Create & Open file by the command:
```shell
nano ghazigram_run.sh
```

then paste this contant in .sh file:
```shell
#!/usr/bin/env bash
cd Ghazigram
python -m ghazigram
```
Then Click `Ctrl+s` and Then `Ctrl+x`


If run Ghazigram then run command in home directory:
```shell
./ghazigram_run.sh
```

All work are done.

Thank You.

**Github**
    
[Ghazigram](https://github.com/inishaikhalishan/Ghazigram)
    
    
[inishaikhalishan](https://github.com/inishaikhalishan)
    
    
**Telegram**

[Ghazigram](https://t.me/ghazigam)


[Ghazigram_Chat](https://t.me/ghazigram_chat)
    

[inishaikhalishan](https://t.me/inishaikhalishan)
    