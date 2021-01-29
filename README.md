# gnome-terminal-settings-backup

You can dump your settings using:
dconf dump /org/gnome/terminal/ > gnome_terminal_settings_backup.txt

Reset (wipe out) the settings before loading a new one (probably not really required):
dconf reset -f /org/gnome/terminal/

Load the saved settings:
dconf load /org/gnome/terminal/ < gnome_terminal_settings_backup.txt
