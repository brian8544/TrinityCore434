## Can I play with my wow.exe of a private server?

Most likely **NO**, unless they are using TCPP core. In order to use this software you need to compile the connection patcher project and use the executable to patch a original wow.exe or wow-64.exe with version 4.3.4.15595. This is because this version of the core uses a different way of communicating with the server than old private servers do.
If you have been able to play with your exe file on other private servers, your exe is not 'clean' and is not compatible for the further steps. You need a clean installation of the client.

## I cannot login

If you fail to login it can have multiple reasons:
1. You have to use battlenet accounts. These accounts are different from regular game accounts. They are created via the bnetaccount create command and usual look similar to this: username@mailadress.
2. You screwed up in the previous steps and did not rename the battle.net-patched.dll properly or you fucked up the auth modules. Check that.
3. You are missing the correct .auth files in C:\Program Data\Blizzard Entertainment\Battle.net
4. realmlist.wtf is no longer used. Instead we use the config.wtf file with the SET portal argument.
5. If you get the invalid version login error you have to delete the original wow launcher from your client directory as it's also being checked on login. Since the launcher is deprecated and useless anyways you can safely delete it.
6. Make sure that your ports are all opened for the connections. Battle.net uses port 1119 and the Worldserver uses the ports 8085 and 8086
7. You may still have Launcher.app/exe inside your Wow folder, delete it

## The patcher did not patch everything

In order to patch successfully all files must be in the same directly of the connection patcher. Once you start patching the wow.exe file it will patch everything directly after that. So make sure everything is there.