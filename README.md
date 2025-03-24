# Steam Achievements for EET
**Version:** v0.1
**Author:** Xarlith

## Description  
This mod allows Steam achievements from **BG1EE, SoD, and BG2EE** to unlock properly during an **EET playthrough**.
Normally, EET is detected as BG2EE, preventing BG1/SoD achievements from unlocking. This mod fixes that by:

- Expanding the **achievements handling script** to include BG1 and SoD in EET.
- Allowing Steam to recognize the **EET game as BG1EE during BG1/SoD** (and switching back to BG2EE for BG2).

## Installation  
This mod uses a **WEIDU installer**. To install:

1. Extract the mod to your **EET installation folder**.
2. Run **setup-eet_achievements.exe**.
3. Select the following components:

   - **"Expanded achievements handler"** → Installs the expanded achievements handling script.
   - **"Set Steam AppID to BG:EE"** → Makes Steam recognize the game as BG1EE.
   - **"Set Steam AppID to BG2:EE"** → Restores normal BG2EE detection when moving to BG2 content.

## How It Works  
- The **modified scripts** allow all achievements (BG1, SoD, and BG2) to trigger properly in EET.
- The **steam_appid.txt file** tells Steam which game is running. By default, it will be set to **BG1EE** when installing this mod.
- **Before entering BG2 (Chateau Irenicus), restore the app ID** using the second component.

## Important Notes
- The **steam_appid.txt file must be placed in the EET main directory** (where `Baldur.exe` is located).
- Make sure you have **steam_api64.dll** in your installation directory—Steam needs it to track achievements.
- **All achievements from your current playthrough may trigger at once** when loading a save, which might look suspicious to Steam.

## Uninstallation
Run **setup-EET_steam_achievements.exe** again and select "Uninstall."

## Future Plans
- Expanding support to include **IWD achievements** in EET/IWD-in-EET mods.
