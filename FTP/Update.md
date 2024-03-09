# Update

### Update Instructions:

1. **Backup:**
   - Make a backup of the `config` and `data` directories in the server files. Optionally, create a backup of all server files in case the update fails.

2. **Database Backup:**
   - Make a backup of the server database (you can use the export feature in phpMyAdmin).

3. **Version Check:**
   - Determine the current version of `database.sql` your server is using. Look for the `Generation Time` on line 6 or use Google Translate if it's in Czech.

4. **Repository Download:**
   - Download a copy of the private server repository from [here](https://github.com/MegaSa1nt/GMDprivateServer).

5. **Configuration Comparison:**
   - Compare the config directory in the new version with your version and edit the files as necessary to set new variables.

6. **File Deletion:**
   - Delete all files from the server EXCEPT for the `config` and `data` directories. (Important: Keep `data` directory to preserve player-made levels).

7. **Upload:**
   - Upload the new server files, including your new config files (if applicable), to the server.

8. **SQL Import:**
   - Import all SQL files in the directory with timestamps newer than your current version `database.sql`. Use the import feature in phpMyAdmin for this.

For detailed instructions, refer to MegaSa1nt's [Update Directory](https://github.com/MegaSa1nt/GMDprivateServer/).
