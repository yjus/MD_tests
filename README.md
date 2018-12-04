# Questions ouvertes
* quelle version d'Abaqus ?
* quelles sont les limitations de la version pédagogique d'Abaqus ?
  * nombre de noeuds ?
  * autre ?



# Modélisation du lâcher de ballon de gym avec Abaqus
La simulation se déroule en 2 étapes :
1. Gonflage
1. Impact

Pour lancer la simulation, tapez `abaqus job=gonflage interactive` puis `abaqus oldjob=gonflage job=impact interactive`dans un terminal.

Les fichiers sont les suivants :
* `elements_ballon.inp` définition des éléments
* `gonflage.inp` gonflage du ballon
* `impact.inp` simulation de l'impact
* `noeuds_ballon.inp` définition des noeuds

# Modélisation du gonflage
Deux méthodes possibles:
* Pression interne
* carte FLUID CAVITY (relation entre la pression et le volume)
