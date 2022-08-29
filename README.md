# adobe-ip-blocker

A hosts file for Windows OS to avoid excessive communication for Adobe apps.

## USAGE

Use only **hosts.csv**. **hosts-default.csv** should be used when you want to restore the hosts file to its initial state.

### Delete the extension

Delete the **.csv** extension.

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

## CAUTION

Back up your hosts file before using it. Updating the hosts file may result in incorrect activation of your Adobe license.
