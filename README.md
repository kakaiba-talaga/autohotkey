# AutoHotkey Scripts

This is a compilation of reusable AHK scripts.

## Requirements

[AutoHotkey](https://www.autohotkey.com/) should be installed first or use a compiled version of the AHK script so it can run by its own.

- AutoHotkey is for **Windows** only.
- Developed and Tested using version `1.1.33.09`.

## AHK Scripts

- [Chrome Profile Launcher](AHK/Chrome-Profile-Launcher.ahk)

    This can launch Chrome instances based on the profile. If the Chrome profile was already launched, it will activate or set the focus to that window.

    ```ahk
    ; CTRL + ALT + ` >>> Open Chrome using the Default profile.
    ^!`::
    chrome_profile_launcher()
    return
    ``

    ```ahk
    ; CTRL + ALT + 1 >>> Open Chrome using the Profile 1 profile.
    ^!1::
    chrome_profile_launcher("Profile 1")
    return
    ```

    Take not that the `DetectHiddenWindows` is turned `On` so the script can check the Chrome window across different virtual desktops.

- [Hotstring Helper](AHK/Hotstring-Helper.ahk)

    This script may be useful if you are a heavy user of *Hotstrings*. It's based on the script originally created by *Andreas Borutta*.

    By pressing the specified *Hotkey*, `CTRL + ALT + H` in this case, the currently selected text can be turned into a *Hotstring*. The newly created *Hotstring* will be appended in the script itself.

    This was customized to be able to add the new *Hotstring* and activate it without reloading the script. In my version, I just made some optimizations.

## Contribute

Community contributions are encouraged! Feel free to report bugs and feature requests to the [issue tracker](https://github.com/kakaiba-talaga/AutoHotkey-Scripts/issues) provided by *GitHub*.

## License

`AutoHotkey` is an Open-Source Software *(OSS)* and is available for use under the [GNU GPL v3](https://github.com/kakaiba-talaga/AutoHotkey-Scripts/blob/main/LICENSE) license.