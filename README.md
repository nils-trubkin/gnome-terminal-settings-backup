# gnome-terminal-settings-backup

You can dump your settings using:
dconf dump /org/gnome/terminal/ > gnome_terminal_settings_backup.txt

Reset (wipe out) the settings before loading a new one (probably not really required):
dconf reset -f /org/gnome/terminal/

Load the saved settings:
dconf load /org/gnome/terminal/ < gnome_terminal_settings_backup.txt

# Font (Source Code Pro)
https://github.com/adobe-fonts/source-code-pro

The directory you're looking for is /usr/share/fonts/opentype. If it's not there, you can just create it. Copy your OTF files there; this will install the font for all users. Then, recreate the fonts cache with the command sudo fc-cache -f -v.

You can also install fonts per user at ~/.fonts/. It makes no difference whether they're in any sub-folders or what type they are. Mine, as an example, are organised by foundry.

Alternatively, you can just double click them, this will open them with the Font Viewer, which let's you install them with one click
