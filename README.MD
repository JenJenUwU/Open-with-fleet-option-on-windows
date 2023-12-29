
# How to add Open with Fleet option in Windows

## Requirements:
- Windows
- Fleet installed

## Procedure
1. Open `Registry Editor` with search bar.
2. Unfold `HKEY_CLASSES_ROOT/*/shell`.
3. Right click on `shell` and select *New > Key* and Name it `Fleet`.
4. On the right side double click `(Default)` and set the value to `Open w&ith Fleet`.
5. Right click `Fleet` and select *New > String Value* and the name to be `Icon` with your path to `Fleet.exe` as the value (Default path is `C:\Users\Your Name\AppData\Local\Programs\Fleet\Fleet.exe`.
6. Right click `Fleet` again and select *New > Key* and Name it `command`.
7. Change the `(Default)` value of `command` to `PATH TO Fleet.exe "%1"` (ex: C:\Users\Your Name\AppData\Local\Programs\Fleet\Fleet.exe "%1").