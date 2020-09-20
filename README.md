# xampp.desktop

---

Create a quick Linux deskotp shortcut/icon for [XAMPP](https://www.apachefriends.org/).

1. Clone or download this repo.

2. Move the xampp.png icon to the default */opt/lampp* directory.
   
   ```bash
   sudo mv xampp.png /opt/lampp/
   ```

3. Move the xampp.desktop file to the *~/.local/share/applications* directory.
   
   ```bash
   sudo mv xampp.desktop ~/.local/share/applications
   ```

4. Edit the *sudoers* file.
   
   ```bash
   sudo visudo
   ```

5. Add the following text to the end of the file. Replace *username* with your username.
   
   ```textile
   username ALL = NOPASSWD: /opt/lampp/manager-linux-x64.run
   ```

6. Make xampp.desktop executable.

7. ```bash
   sudo chmod +x ~/.local/share/applications/xampp.desktp
   ```
