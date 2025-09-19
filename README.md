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
- `FirstItemReceivedTimespan` is the amount of time in seconds the mod will wait for the first transfered item to be added to player's inventory. On a regular Nitrado server the transfered items should be added to player's inventory less than 1 second after player character has spawned. This is set to `10` seconds by default to allow for some flexibility. Minimum value is `5`, maximum value is `60`.
- `ReceivingItemsTimespan` is the amount of time in seconds the mod will check for duplicates when an item gets added to player's inventory. On a regular Nitrado server the items transfer should take around a second. This is set to `8` seconds by default to allow for some flexibility. Minimum value is `5`, maximum value is `60`.

You can refer to the following picture if you want to understand how the timespan settings work. The picture shows what happens when a player spawns (after a map travel):
![Nitrado Transfers Fix timespan settings image](https://i.imgur.com/V8M5SRY.png)


# Info & Support

Please use the comments section of this mod on CurseForge if you need information and/or support:<br>
[https://www.curseforge.com/ark-survival-ascended/mods/nitrado-transfers-fix](https://www.curseforge.com/ark-survival-ascended/mods/nitrado-transfers-fix)<br>
Or join my Discord server:<br>
https://discord.gg/PtAbeUdWX8

<br>
