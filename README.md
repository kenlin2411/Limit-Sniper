- [LimitSwap](#sniper)
  * [HOW TO INSTALL Sniper](#how-to-install-sniper)
    + [1. Run The Python Code Locally](#1-run-the-python-code-locally)
      - [For Windows users](#for-windows-users)
      - [For Linux users](#for-linux-users)
      - [For Mac users](#for-mac-users)
    + [2. Download the pre-compiled package (For Windows users only)](#2-download-the-pre-compiled-package-for-windows-users-only)



# Sniper
A mempool sniping bot for Ethereum, Binance Smart Chain, Matic, & Fantom that is able to scan for new liquidity adds on token launches, so as to be able to buy a token as soon as liquidity is added --> in the same block


&nbsp;
&nbsp; 

## HOW TO INSTALL Sniper
There are 2 ways to install : 

&nbsp;

### 1. Download the pre-compiled package for Windows users only

That we provide on the Release page : it's a .exe file that you can run on your computer.
https://github.com/tsarbuig/Limit-Sniper/releases


- [x] Download last Zip file, for instance :

<img src="https://user-images.githubusercontent.com/70858574/145737351-c659185f-e1f5-4ede-b81e-3b03d0f900f9.png" width="200">

- [x] Unzip it
- [x] Open "tokens.json - Shortcut" and configure it for your needs
- [x] Open "Start Sniper.cmd" --> it will configure your settings.json

✅ ✅ ✅ And it's done! ✅ ✅ ✅

&nbsp; 

#### Pros and cons
🟢 : very easy to setup

🔴 : it's pre-compiled, so you cannot check the Source Code

&nbsp;
&nbsp;


### 2. Run The Python Code Locally 
Here are tutorials step-by-step: 

&nbsp;

#### For Windows users

----------------------------------------

**FIRST PART : PRE-REQUISITES** 

----------------------------------------

- [x] Install Python on your computer : https://www.python.org/downloads/ 

**PLEASE ADD IT TO PATH BY CHECKING THIS OPTION:**

<img src="https://user-images.githubusercontent.com/70858574/145738124-e724c843-82d5-410d-b0b4-d7a9dda92258.png" width="500">

- [x] Install Visual Studio : https://visualstudio.microsoft.com/thank-you-downloading-visual-studio/?sku=Community&rel=17

Please install the default package and all those options :
![image](https://user-images.githubusercontent.com/70858574/145580447-bd648d6d-c3ce-4dd9-8527-84ecfb5f30cc.png)

- [x] NEW : Sniper now has colors to better display errors / success / etc. 

Follow this tutorial to activate colors on your Windows Command :
  - 1/ Launch "Regedit"
  - 2/ Go to [HKEY_CURRENT_USER \ Console]
  - 3/ Right click on white space / create new DWORD 32 bit key called `VirtualTerminalLevel` and set it to 1

<img src="https://user-images.githubusercontent.com/70858574/148842282-285a4c22-a569-44f3-9b93-ee7ff951c6ff.png" width="500">

&nbsp;

----------------------------------------

**SECOND PART : DOWNLOAD BOT AND INSTALL DEPENDENCIES** 

----------------------------------------

- [x] Download last Sniper code on the "Code" page https://github.com/tsarbuig/Limit-Sniper by clicking on Code > Download Zip : 
<img src="https://user-images.githubusercontent.com/70858574/148130738-ef447465-511a-41b8-bcf2-6766a41fdbb8.png" width="300">


- [x] Unzip file
  - [X] Go into the unzipped folder
  - [X] In the folder, push "Shift" on your keyboard, then do a right-click
  - [X] Click on "Open command windows here" or "Open Powershell windows here"
  
<img src="https://user-images.githubusercontent.com/70858574/148840931-ed9ae3d8-e045-43a8-a000-2a52e6f2b4c5.png" width="700">


- [x] It will open Windows command (or Powershell) in the right place, where all the files are located:

![image](https://user-images.githubusercontent.com/70858574/148841299-bfa53046-a8c5-4dd9-9fbe-dddc8f76877e.png)


- [x] Run command: `pip install -r requirements.txt`  
--> this will install all the packages needed to run LimitSwap


(🔥 if you have an error here, double check you have selected "Add Python to PATH" on the Python step. If you did not, uninstall Python and reinstall it checking the option "Add Python to PATH")

&nbsp;

✅ ✅ ✅ And it's done! ✅ ✅ ✅

&nbsp;

----------------------------------------

**LAST PART : RUN THE BOT** 

----------------------------------------
There are 2 ways to do that : 

- [x] Simply **double-click on "sniper.py"** and it will run, since you've installed Python 👍👍

- [x] Or, in the Windows Command, run command: `python sniper.py`  

This second option allows you to use parameters. For example, if you have several .json files and you want to choose which one to use :

`python sniper.py -s settingsBSC.json -t tokensBSC.json`  

or

`python sniper.py --benchmark`  

&nbsp;
&nbsp;

#### For Linux users

----------------------------------------

DO THIS ONCE

----------------------------------------


 `sudo -s`

 `apt-get install python3-dev build-essential python3-pip`


----------------------------------------

DO THE NEXT STEPS FOR EACH UPGRADE

----------------------------------------

Navigate to the Limistswap folder, then:

`python3 -m venv env`

`source env/bin/activate`

`pip install wheel`

`pip install -r requirements.txt`

`python sniper.py`

This allows you to use parameters. For example, if you have several .json files and you want to choose which one to use :

`python sniper.py -s settingsBSC.json -t tokensBSC.json`  

or

`python sniper.py --benchmark`  

&nbsp;

#### For Mac users

----------------------------------------

Tutorial is almost the same as [Windows tutorial](#for-windows-users) 

Check Windows tutorial for detailed step-by-step

----------------------------------------

1/ Install Python and don't forget to select "Add to path"

2/ Install Visual Studio

3/ Open Terminal, go to the directory where you unzipped the bot, and run command: 

`pip install -r requirements.txt`  

&nbsp;

✅ ✅ ✅ And it's done! ✅ ✅ ✅

----------------------------------------

**LAST PART : RUN THE BOT** 

----------------------------------------

Open Terminal, go to the directory where you unzipped the bot, and run command: `python sniper.py`  

&nbsp;

This allows you to use parameters. For example, if you have several .json files and you want to choose which one to use :

`python sniper.py -s settingsBSC.json -t tokensBSC.json`  

or

`python sniper.py --benchmark`  

&nbsp;&nbsp;
&nbsp;



## Developers 🔧
Want to help contribute to LimitSwap, reach out on telegram : any help is welcome to make the bot better  :)


## Links & Socials

#### WiKi
https://limitswapv3.gitbook.io/limitswap/

#### Website:
https://www.limitswap.com/

#### Twitter:
https://twitter.com/LimitSwap

#### Telegram:
https://t.me/LimitSwap
