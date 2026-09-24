# Windows Basic Caption Buttons

Restores classic, rectangular Windows Basic non-client caption buttons directly within Desktop Window Manager (`dwm.exe`) without relying on external theme engines like Basic Themer.

## Why Use This Instead of Basic Themer?

Most Windows 7 / Basic themes rely on **Basic Themer**, which introduces well-known stability issues across modern Windows builds:
* **No Basic Themer crashes:** Avoids UI glitches, app freezes, and desktop crashes caused by hook injection.
* **Full DWM Compatibility:** Keeps DWM running smoothly without breaking transparency or system animations.
* **Proper Window Scaling:** Caption buttons remain accurately aligned and sized across standard app windows and DWM-required textboxes.

## Prerequisites for the Full Basic Look

To get the complete Windows Basic visual experience, set up the theme files first:

1. **Theme Engine Patcher:** Install [SecureUxTheme](https://github.com/namazso/SecureUxTheme) or [UltraUxThemePatcher](https://mhoefs.de/software/uxthemepatcher/en/index.php) to enable custom visual styles.
2. **Basic Visual Style:** Download and apply the [Aero10 (Vista/Seven) Theme by vaporvance](https://www.deviantart.com/vaporvance/art/Aero10-Vista-Seven-909711949).
3. **OpenGlass:** Download and Launch the [OpenGlass Latest Version](https://github.com/ALTaleX531/OpenGlass/releases/tag/v3.0.1.3747).

## ⚠️ Important: Process Inclusion List Required
`dwm.exe` is on Windhawk's critical system process list. Because of this, **you must add `dwm.exe` to the process inclusion list** in Windhawk's Advanced settings (`Settings -> Advanced settings -> More advanced settings`), otherwise the mod will silently fail to inject and won't work.

---

## Installation Options

### Option 1: Automated Helper Tool (Recommended)
You can use the helper executable included in the repository to simplify installation and keep your mod updated:
1. Download and run `GIT-WBCB-INSTALLER.exe` from the latest release.
2. The tool checks GitHub for the latest version of the C++ mod code and opens Windhawk with the code ready for compilation.
3. In Windhawk, click **Compile / Accept** to finish installing.

---

### Option 2: Manual Installation
1. Open **Windhawk** and go to **Explore** → **Create a new mod**.
2. Copy the code from `restore-basic-caption-buttons.wh.cpp` in this repository.
3. Paste the code into the Windhawk editor replacing any existing text.
4. Ensure `dwm.exe` is on your Process Inclusion list, then click **Compile / Accept**.

---

## Compatibility
* **Windows 10:** Confirmed working on **21H2** and older builds (such as **1903+**).
* **Windows 11:** Not supported due to major non-client layout changes in DWM.
