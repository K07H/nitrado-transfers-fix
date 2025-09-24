# Description

Nitrado Transfers Fix is a mod for Ark Survival Ascended.<br>
This mod fixes the inventory duplication bug that can occur when travelling to another map on Nitrado servers.<br>
A lot of people have been complaining about this bug (including myself), and since after 2 years the issue has not been fixed I decided to make the fix myself.<br>
<br>
<strong>Author:</strong> OSubMarin<br>
_If you like this mod please consider donating: [https://paypal.me/osubmarin](https://paypal.me/osubmarin)_<br>



# Configuration

This mod is correctly configured by default and therefore does not require any changes to the GameUserSettings.ini file.<br>
However, you can modify certain settings by adding the following lines to the end of your GameUserSettings.ini file:

```
[NitradoTransfersFix]
FixTransfersDupes=True
EnableLogging=False
LogAllEvents=False
FirstItemReceivedTimespan=60
ReceivingItemsTimespan=60
```



# Explanations

- `FixTransfersDupes` can be set to `False` if you want to turn OFF the mod without uninstalling it.
- `EnableLogging` can be set to `True` if you want the mod to add logging lines in the `ShooterGame.log` file. If set to `True`, only "player joined" and "amount of transfered items" events will be logged, but more things can be logged if you also set `LogAllEvents` to `True`.
- `LogAllEvents` can be set to `True` if you want to add additional logging lines in the `ShooterGame.log` file. Has no effect if `EnableLogging` is not set to `True`. Setting this to `True` is not recommended unless for testing purposes. This will log all the operations made by the mod when a player receives a transfered item.
- `FirstItemReceivedTimespan` is the amount of time in seconds the mod will wait for the first transfered item to be added to player's inventory. You should not modify this value. Default value is `60` seconds, minimum value is `5`, maximum value is `180`.
- `ReceivingItemsTimespan` is the amount of time in seconds the mod will check for duplicates when an item gets added to player's inventory. You should not modify this value. Default value is `60` seconds, minimum value is `5`, maximum value is `180`.

### About `FirstItemReceivedTimespan` and `ReceivingItemsTimespan`

On a regular Nitrado server you should not modify the values of `FirstItemReceivedTimespan` and `ReceivingItemsTimespan`.<br>
If some item duplication is still happening with this mod installed, it's probably because your Nitrado server is extremely slow at processing map travels, which is not normal.<br>
If your Nitrado server is extremely slow at processing map travels you can try to increase `FirstItemReceivedTimespan` and `ReceivingItemsTimespan` values.<br>
You can refer to the following picture if you want to understand how these two settings work. The picture shows what happens when a player spawns (after a map travel):
![https://i.imgur.com/3iXl8C2.png](https://i.imgur.com/3iXl8C2.png)



# Loading in Ark Survival Ascended DevKit

To load the mod in ARK Survival Ascended DevKit, simply copy the folder `NitradoTransfersFix` inside folder `[...]\Epic Games\ARKDevkit\Projects\ShooterGame\Mods`.
Then launch the DevKit, open the level of your choice (`TestMapArea` by default), and set `PrimalGameData_BP_NitradoTransfersFix` in the level's `Primal Game Data Override` setting (`World Settings` tab).



# Info & Support

Please use the comments section of this mod on CurseForge if you need information and/or support:<br>
[https://www.curseforge.com/ark-survival-ascended/mods/nitrado-transfers-fix](https://www.curseforge.com/ark-survival-ascended/mods/nitrado-transfers-fix)<br>
Or join my Discord server:<br>
https://discord.gg/PtAbeUdWX8

<br>
