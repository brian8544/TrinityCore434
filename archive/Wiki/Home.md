# Welcome to the TrinityCore 4.3.4.15595 wiki
This page is going to address all TCPP related information.

Please check https://trinitycore.info/ for general information about TrinityCore (e.g. setup).

## I need a full client
Please check [I need a full client](https://github.com/The-Cataclysm-Preservation-Project/TrinityCore/wiki/I-need-a-full-client)

**Windows only note: If you followed the "I need a full client" part, you can skip following part!**

Both Windows and MacOS need a valid WoW.mfil in the World of Warcraft root dir with following content:
```
version=2
server=akamai
    location=http://dist.blizzard.com.edgesuite.net/wow-pod-retail/EU/15050.direct/
manifest_partial=wow-15595-0C3502F50D17376754B9E9CB0109F4C5.mfil
```
Make sure you protect the file from changes by setting write protection (Windows) or locked (MacOS)

## How to connect using connection_patcher
Please check [connection_patcher](https://github.com/The-Cataclysm-Preservation-Project/TrinityCore/wiki/connection_patcher)


## How to connect using client_launcher and client_patcher (WINDOWS ONLY!)
_**Note 1:** client_launcher_32 will **only** run 32bit Wow and client_launcher_64 **only** 64bit Wow_

_**Note 2:** You need client_launcher_XX.exe **AND** client_patcher_XX.dll_

_**Note 3:** You may need to copy some OpenSSL dlls too_

_**Note 4:** You need to start Wow with launcher all the time to be able to play on TCPP_

**REQUIRED:** To connect to server you need to edit Config.WTF in WTF folder! (realmlist.wtf is not a thing in this project anymore)

`SET portal "127.0.0.1"`

Step 1: Get Clean Wow.exe and Battle.net.dll or the 64bit version

Step 2: Make sure there is no original Launcher.exe inside WoW folder

Step 3: Get client_launcher_32.exe and client_patcher_32.dll or client_launcher_64.exe and client_patcher_64.dll and place them into wow folder.

Step 4: Run client_launcher

**Additional options:** 

--console (displays client_patcher console (it's the AllocConsole of Wow Process)

--path -> path to Wow folder if launched outside wow folder

## Troubleshooting
Please check [Troubleshooting](https://github.com/The-Cataclysm-Preservation-Project/TrinityCore/wiki/Troubleshooting)