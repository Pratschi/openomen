## 🖥️ Make a Desktop Shortcut

1. Open a terminal and navigate to the applications folder:

```bash
cd /usr/share/applications
sudo nano openomen.desktop
```
Paste the following content (update paths as needed):
```bash
[Desktop Entry]
Version=1.0
Type=Application
Name=OpenOMEN Hub
Exec=sudo /home/yourusername/path/to/OpenOMEN-x86_64.AppImage
Terminal=false
StartupNotify=true
Categories=Utility;
```
> Replace /home/yourusername/... with the actual path to your AppImage and icon.

2. Allow launching without a password

Edit sudoers using visudo:
```bash
sudo visudo
```
Add the following line at the end (replacing with your actual username):
```bash
yourusername ALL = NOPASSWD: /home/yourusername/path/to/OpenOMEN-x86_64.AppImage
```

## 📂 Launch from Applications Menu
After completing the steps above, you can now find **OpenOMEN Hub** in your Applications menu and launch it like any other app. **(You might have to restart your desktop database in most cases.)**
```bash
sudo update-desktop-database
```