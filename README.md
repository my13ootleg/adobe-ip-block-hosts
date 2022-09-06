# Overview

A hosts file for Windows OS to avoid excessive communication for Adobe apps.

## Confirmed apps
The following apps have confirmed this.

- After Effects 22.1
- Animate 22.0
- Audition 22.1
- Character Animator 22.1
- Dreamweaver 21.1
- Fresco 3.8
- Illustrator 26.0
- InDesign 17.0
- Lightroom 4.2
- Photoshop 23.1
- Premiere Pro 22.1
- XD 47.0

## Usage

Use only **hosts**. **hosts-default** should be used when you want to restore the hosts file to its initial state.

### Overwrite hosts file

Access the following directory in Windows Explorer.

```
C:\Windows\System32\drivers\etc
```

Overwrite the hosts file.

## Use without overwriting the hosts file

The hosts file can be additioned to rather than overwritten.

1. Open the file `C:\Windows\system32\drivers\etc\hosts` with a code editor such as [VSCode](https://azure.microsoft.com/ja-jp/products/visual-studio-code/).
2. Add to the last line.
3. Ctrl+S to save.
4. Make sure it does not have an extension such as **.txt**. If the extension is attached, delete it.

## Caution

Back up your hosts file before using it. Updating the hosts file may result in incorrect activation of your Adobe license. If you encounter problems, you can restore the hosts file to its initial state by overwriting it with **hosts-default**.
