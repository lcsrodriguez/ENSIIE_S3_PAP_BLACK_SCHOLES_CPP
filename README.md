
# Projet PAP

## Introduction


## Commande
Commande pour exécuter le programme
```
cd source
rm projet
g++ -g -Wall -Wextra -o projet *.cpp `pkg-config --cflags --libs sdl2 sdl2_ttf`
./projet
```

**Remarque** : La librairie __sdl2_ttf__ a été ajouté à la clause pkg-config afin de pouvoir gérer l'affichage de texte

## Licence

Lucas RODRIGUEZ