# How to Install UBL

Follow these steps to install the **UBL** and start using it in your game.

## UBL is no longer supported nor maintained. If you encounter issues while using it, you are on your own.

---

## ⚠️ **Pre-Requisites**
Before installing UBL, you must have the **[MK12TTH](https://www.nexusmods.com/mortalkombat/mods/62)** installed.  

---

## **Step 1: Download UBL**
1. Download the latest **[UBL](https://www.nexusmods.com/mortalkombat/mods/1138/)**.
2. Locate your **game’s root folder**:
   - **Steam:** Right-click **Mortal Kombat 1** → **Manage** → **Browse Local Files**.

---

## **Step 2: Extract and Install UBL**
1. Extract the downloaded **UBL archive**.
2. Move **all extracted folders** into your **game’s root folder**.

 **At this point, UBL is installed, but you still need to configure the game to use it!**

---

##️ **Step 3: Configure the Game to Use UBL**
You must tell the game to use the **UBL instances** instead of the default ones.

1. **Navigate to your game's local appdata folder:**  
   - **Press `Win + R`** and paste one of the following paths, depending on your platform:

   - **Steam Version:**
     ```
     %localappdata%/MK12/Saved/Steam/Config/WindowsNoEditor
     ```
   - **Epic Games Store Version:**
     ```
     %localappdata%/MK12/Saved/EOS/Config/WindowsNoEditor
     ```

2. **Open `Engine.ini`** in a text editor.
3. **Paste the following lines at the very bottom:**
   ```
   [/Script/EngineSettings.GameMapsSettings]
   GlobalDefaultGameMode=/Game/UBL/UBLMapModeGameMode.UBLMapModeGameMode_C
   GameInstanceClass=/Game/UBL/UBLFightingGameInstance.UBLFightingGameInstance_C
   ```
   
## How to Install UBL Mods

UBL mods must be placed in the following directory inside your game’s folder:

```
MK12/Content/Paks/BPMods
```

### **Steps to Install a Mod**
1. **Download a UBL-compatible mod.**  
2. **Extract the mod files** 
3. **Move the following files into the `BPMods` folder**:
   - `.pak`
   - `.ucas`
   - `.utoc`

**The mod should now be loaded when you launch the game.**