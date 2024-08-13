## Required Actions
To connect to server you need to edit Config.WTF in WTF folder! (realmlist.wtf is not a thing in this project anymore)

`SET portal "127.0.0.1"`
## Windows:
You have to patch the following game components:
* the Wow.exe or Wow-64.exe
* the Battle.net.dll or Battle.net-64.dll (happens automatically)
* the Wow authentication modules which will be downloaded and patched by the connection patcher itself. If the connection patcher should somehow fail to retrieve the auth modules, you can find a backup dump of the modules here:
https://github.com/The-Cataclysm-Preservation-Project/AuthModules

1. You have to download all modules by yourself.
https://github.com/The-Cataclysm-Preservation-Project/AuthModules/tree/master/Windows
The path must be exactly the same "C:/ProgramData/Blizzard Entertainment/Battle.net/Cache/..." as represented in the repository.
2. Get a **Clean** Wow.exe and a **clean** Battle.net.dll (4.3.4.15595) and/or Wow-64.exe and Battle-64.net.dll (look at 'I need a full client') !!! DO NOT HAVE THEM IN USERS FOLDER (e.g. C:/Users/braindead/Wow) CHOOSE A PATH LIKE C:/Games/WoW/ !!!
3. Drag Wow.exe and/or Wow-64.exe on connection_patcher
4. Check log if everything worked
5. Rename the existing Wow.exe and Battle.net.dll and/or Wow-64.exe and Battle-64.net.dll 
OR 
move them to another folder
6. Rename the Wow_patched.exe and the Battle.net_patched.dll and/or the Wow-64_patched.exe and Battle-64.net_patched.dll
to: Wow.exe Battle.net.dll Wow-64.exe Battle-64.net.dll
7. If you have a Launcher.exe rename it into something else (e.g. Launcher-Backup.exe)

## MacOS:
You have to patch the following game components:
* the 'World of Warcraft-64.app' (in fact the components inside are being patched)
* the Wow authentication modules which will be downloaded and patched by the connection patcher itself. If the connection patcher should somehow fail to retrieve the auth modules, you can find a backup dump of the modules here:
https://github.com/The-Cataclysm-Preservation-Project/AuthModules

1. Get a **clean** 'World of Warcraft-64.app' (look at 'I need a full client')
2. Open Terminal and drag connection_patcher on it and after that the 'World of Warcraft-64.app' and hit Return/Enter.
3. Check log if everything worked
4. Rename the existing 'World of Warcraft-64.app'
OR 
move them to another folder
5. Rename 'World of Warcraft-64_patched.app' to 'World of Warcraft-64.app'
6. If you have a Launcher.app rename it into something else (e.g. Launcher-Backup.app)
7. Go to '/Users/Shared/Blizzard/Battle.net/Cache/19/c9/' folder and locate the '19C91B68752B7826DF498BF73ACA1103C86962A9A55A0A7033E5AD895F4D927C.auth' file
8. Rightclick and select 'Get Info' and check 'Locked' 

![Screenshot 2022-02-24 at 01 21 42](https://user-images.githubusercontent.com/846960/155433263-ab66580c-143e-43a4-ab69-740f24825fbd.png)
**This is important!**

## Linux:
Linux is not officially supported. But there are people who are running it on wine. Ask in the discord.

## I have patched everything, what now?

Once the patching is complete you should have a Wow-patched.exe or a Wow-64-patched.exe as well as a battle.net-patched.dll or a battle.net-64-patched.dll. If that is the case, delete the original battle.net.dll and replace it with the patched version. Once it's done you are set to go
