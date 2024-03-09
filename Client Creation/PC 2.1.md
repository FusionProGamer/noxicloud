# PC 2.1

**Taken From GMDprivate server by [Cvolton](https://github.com/Cvolton)**

# Programs

- [HxD](https://mh-nexus.de/en/downloads.php?product=HxD20)
- [GD 2.1](http://www.mediafire.com/file/zvy1554tsdd2qd6/Geometry_Dash_2.11_PC.zip/file)

**Now Follow These Steps:**

1. Open `geometrydash.exe` with HxD Portable.
2. Search for `http://www.boomlings.com/`.
3. Replace it with your root link.
   - Example: `http://fusion.noxicloud.es/` (Exact letter count required)
   - Note: If you have an additional folder in your link, search your link before `database/`.
4. Search for `aHR0cDovL3d3dy5ib29tbGluZ3MuY29tL2RhdGFiYXNlL3` (Base64 Encoded: `http://www.boomlings.com/database/`).
5. Change it with your root link encoded with base64 including `database/`.
   - Example: `http://fusion.noxicloud.es/database/` -> `aHR0cDovL2dkcHMuZW1yZW95dW4uY29tL2RhdGFiYXNlL3` (Base64 encoded).
   - Note: If you encounter an error about size change, remove the last "w==" and add "3".
6. Search for `aHR0cDovL3d3dy5ib29tbGluZ3MuY29tLw==` (Base64 Encoded: `http://www.boomlings.com/`).
7. Change it with your root link encoded with Base64.
   - Example: `http://fusion.noxicloud.es/` -> `aHR0cDovL2dkcHMuZW1yZW95dW4uY29tLw==` (Base64 encoded).
   - Note: If you encounter an error about size change, remove the last "w==" only.
8. Save the file as `yourgdpsname.exe`.
9. Run and profit!!!
