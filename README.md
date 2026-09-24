# Windows Basic Caption Buttons

Restores classic, rectangular Windows Basic caption buttons directly within Desktop Window Manager (`dwm.exe`) without relying on external theme engines like Basic Themer.

## Why Use This Instead of Basic Themer?

Most Windows 7 / Basic themes rely on **Basic Themer**, which introduces well-known stability issues across modern Windows builds:
* **No Basic Themer crashes:** Avoids UI glitches, app freezes, and desktop crashes caused by hook injection.
* **Full DWM Compatibility:** Keeps DWM running smoothly without breaking transparency or system animations.
* **Proper Window Scaling:** Caption buttons remain accurately aligned and sized across standard app windows and DWM-required textboxes.

## ⚠️ Important: Process Inclusion List Required
`dwm.exe` is on Windhawk's critical system process list. Because of this, **you must add `dwm.exe` to the process inclusion list** in Windhawk's Advanced settings, otherwise the mod will silently fail to inject and won't work.

## How to Install (Local Mod)
1. Open **Windhawk** and go to your local mods or click to create a new advanced/local mod.
2. Copy the code from the `restore-basic-caption-buttons.wh.cpp` file in this repository.
3. Paste the code into the Windhawk editor.
4. Make sure `dwm.exe` is added to your Process Inclusion list, then click **Compile / Accept**.

## Compatibility
* **Windows 10:** Confirmed working on **21H2** and older builds (such as **1903+**).
* **Windows 11:** Not supported due to major non-client layout changes in DWM.
