# Android 2.1

**Taken From GMDprivate server by [Cvolton](https://github.com/Cvolton)**

**You will be needing:**
- [APK Editor](http://emreoyun.keybase.pub/APK-Editor-Pro-1.9.7-emreoyun.com.apk)
- [Geometry Dash 2.1](http://www.mediafire.com/file/1flou0h22z0djrc/Geometry_Dash_2.111.apk/file)
- [Hex Editor](http://www.mediafire.com/file/9wq0p4hxhcqfhv8/HEX_Editor_v2.8.1_apkpure.com.apk/file)

**Steps:**

1. Download the GD APK file and open it with Apk Editor Pro, then select simple edit.
2. Go to `lib` and `armabi` folder, then save the `libcocos2dcpp.so` file by tapping the floppy disk icon. Ensure you save it in a known location.
    - Example: `/sdcard0/GDPStest`
3. Close the app, reopen it, and select common edit.
4. Change the package name to something different from the original GD.
    - Example: `com.robtopx.geometryjump` to `com.gdpssxx.yourgdpsname`
    - Note: Ensure the new package name has the same length as the old one.
5. Optional: Rename the app if desired.
6. After changing the package name, tap Save and wait for the process to complete.
7. Once successful, go to the location of the app, rename it to prevent replacement, but keep `.apk`.
    - Location: `/sdcard/ApkEditor/tmp/gen_signed.apk`
    - Example: `gdpstestgen_signed.apk`
8. Open HEX Editor and open `libcocos2dcpp.so`.
9. Search for `http://www.boomlings.com/` and replace it with your root link.
    - Example: `http://gdps.emreoyun.com/`
    - Note: If you have additional folders in your link, search the link before `database/`.
10. Search for `aHR0cDovL3d3dy5ib29tbGluZ3MuY29tL2RhdGFiYXNlLw==` (Base64 encoded: `http://www.boomlings.com/database/`) and replace it with your root link encoded with base64 including `database/`.
    - Example: `http://gdps.emreoyun.com/database/` -> `aHR0cDovL2dkcHMuZW1yZW95dW4uY29tL2RhdGFiYXNlLw==`
11. If you encounter a size change error, remove the last "w==" from the encoded link and add "3".
12. Search for `aHR0cDovL3d3dy5ib29tbGluZ3MuY29tLw==` (Base64 encoded: `http://www.boomlings.com/`) and replace it with your root link encoded with base64.
    - Example: `http://gdps.emreoyun.com/` -> `aHR0cDovL2dkcHMuZW1yZW95dW4uY29tLw==`
13. If you encounter a size change error, remove the last "w==" from the encoded link and add "2".
14. Search for the app package name and replace it with your package name.
    - Example: `com.robtopx.geometryjump` to `com.gdpssxx.yourgdpsname`
15. Save by tapping the floppy disk icon.
16. Open APK Editor Pro and find the renamed file.
17. Open `gdpstestgen_signed.apk` and select simple edit.
18. Go to `lib` and `armabi`, then replace `libcocos2dcpp.so` with the new one.
    - Location: `sdcard0/GDPStest`
19. Save and wait for the process to complete; it will be named `gen_signed.apk` again.
20. After waiting, install `gen_signed.apk` and test it. If it works, good job! 😄

**Notes:**
- Normal Website (32 items replaced)
- Encoded Website (22 items replaced)
- Package Name (3 items replaced)
- If it says 1, you didn't replace them all.
