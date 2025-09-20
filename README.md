# Description

Nitrado Transfers Fix is a mod for Ark Survival Ascended.<br>
This mod fixes the inventory duplication bug that can occur when travelling to another map on Nitrado servers.<br>
A lot of people have been complaining about this bug (including myself), and since after 2 years the issue has not been fixed I decided to make the fix myself.<br>
If you like this mod please consider donating: [https://www.paypal.com/paypalme/osubmarin](https://www.paypal.com/paypalme/osubmarin)<br>
<br>
<strong>Version:</strong> 1.0<br>
<strong>Author:</strong> OSubMarin



# Configuration

Add the following at the end of your `GameUserSettings.ini` file:

```
[NitradoTransfersFix]
EnableLogging=True
FixTransfersDupes=True
FirstItemReceivedTimespan=10
ReceivingItemsTimespan=8
```



# Explanations

- `EnableLogging` can be set to `False` if you don't want the mod to add lines in the `ShooterGame.log` file.
- `FixTransfersDupes` can be set to `False` if you want to turn OFF the mod.
- `FirstItemReceivedTimespan` is the amount of time in seconds the mod will wait for the first transfered item to be added to player's inventory. This is set to `60` seconds by default to allow for some flexibility. Minimum value is `5`, maximum value is `120`.
- `ReceivingItemsTimespan` is the amount of time in seconds the mod will check for duplicates when an item gets added to player's inventory. This is set to `60` seconds by default to allow for some flexibility. Minimum value is `5`, maximum value is `120`.

You can refer to the following picture if you want to understand how the timespan settings work. The picture shows what happens when a player spawns (after a map travel):
![https://i.imgur.com/3iXl8C2.png](https://i.imgur.com/3iXl8C2.png)



# Loading in Ark Survival Ascended DevKit

To load the mod in Ark Survival Ascended DevKit, simply copy the folder `NitradoTransfersFix` inside folder `[...]\Epic Games\ARKDevkit\Projects\ShooterGame\Mods`.
Then launch the DevKit, open the level of your choice (`TestMapArea` by default), and set `PrimalGameData_BP_NitradoTransfersFix` in the level's `Primal Game Data Override` setting (`World Settings` tab).



# Info & Support

Please use the comments section of this mod on CurseForge if you need information and/or support:<br>
[https://www.curseforge.com/ark-survival-ascended/mods/nitrado-transfers-fix](https://www.curseforge.com/ark-survival-ascended/mods/nitrado-transfers-fix)<br>
Or join my Discord server:<br>
https://discord.gg/PtAbeUdWX8

<br>
