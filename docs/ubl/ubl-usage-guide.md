# Using UBL in Your Mod

This guide explains how to **integrate the UBL framework** into your MK1 mods.

## UBL is no longer supported nor maintained. If you encounter issues while using it, you are on your own.

---

## **1. Download the UBLSampleProject**
To begin integrating **UBL** into your mod, **download the [UBLSampleProject](https://github.com/MK1-Modding/SampleUBLProject)**.
This project contains **pre-made UBL events**, making it easy to get started.

### **Tip:** Adding UBL to an Existing Project
If you're adding UBL to an existing **Unreal Engine project**, simply **copy** the following folder into your project's `Content` directory:

``
Content/CustomBlueprint
``

This folder contains a **sample mod actor blueprint** that already supports UBL events.

---

## **2. Open the UBL Sample Blueprint**
1. **Open your Unreal Engine project.**
2. **Navigate to the** `Content/CustomBlueprint` **folder**.
3. Locate the **SampleBlueprintMod** actor blueprint—this is where all UBL logic happens.

---

## **3. Understanding the Sample Blueprint**
The sample blueprint contains an example usage of the **ChangeFace** event.

**For a full list of UBL events and how to use them, check the** [Events Overview](events/events-overview.md) **section.**

---

## **4. Adding UBL Events to Your Mod**
To add a new UBL event in your mod:

1. Open `SampleBlueprintMod`.
2. **Find the `Event BeginPlay` node.**  
   - If you **have no events yet**, drag off from the **`exec` pin** of `Event BeginPlay`.
   - If you **already have an event**, drag off from its output pin.
3. **Search for the event you want to add** and create it.
4. **Connect it to your event chain.**

 **UBL events should be called in a sequence, forming an event chain.**  

---

## **5. Saving & Compiling the Blueprint**
Once you're done adding UBL events:

1. **Click the "Compile" button** (top-left of the blueprint editor) to save changes.
2. **Ensure the blueprint is named correctly:**
   - **Your blueprint name must match your mod's `.pak`, `.ucas`, and `.utoc` file names.**
   - Example: If your mod files are named:
     ```
     MyCustomBlueprint.pak
     MyCustomBlueprint.ucas
     MyCustomBlueprint.utoc
     ```
     Then your blueprint **inside `CustomBlueprint/` must also be named**:
     ```
     MyCustomBlueprint
     ```
