# Gnome

## Gnome Tweakings 

- Ecran secondaire pris en compte pas les bureaux virtuels : Tweaks (gnome 3) -> espace de travail -> "les espaces de travail couvrent les écrans"
ou gsettings "set org.gnome.mutter workspaces-only-on-primary false"

- gsettings set org.gnome.shell.app-switcher current-workspace-only true -> pour que le alt tab ne montre que les applis du bureau virtuel actif