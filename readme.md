https://unix.stackexchange.com/questions/448811/how-to-export-a-gnome-terminal-profile

source system:

```
$ dconf dump /org/gnome/terminal/legacy/profiles:/ > gnome-terminal-profiles.dconf
```

destination system (after transferring the gnome-terminal-profiles.dconf file):

```
$ dconf load /org/gnome/terminal/legacy/profiles:/ < gnome-terminal-profiles.dconf
```
