# VMMgr
Simple script bash pour gérer des machines virtuelles sous Qemu/Kvm

La définition des machines virtuelles s'appuyent sur des templates, qui peuvent tous être personnalisés.

Pour créer une machine virtuelle, lancer simplement:

./VMMgr_Launcher create linux-base MyVM

Cela va copier le template linux-base dans VM-Availables, en personnalisant quelques variables comme le nom de la vm.

Cette copie peut donc être personnalisé, puis démarré:

./VMMgr_Launcher start MyVM

il est possible d'accéder à la VM en utilisant SPICE, un fichier est créé dans R-SPICE
L'accès à la VM peut se faire de différentes manières:

./VMMgr_Launcher connect telnet MyVM

pour un accès telnet, mais un accès qmp et spice sont également possible

Pour arrêter une VM:

./VMMgr_Launcher stop MyVM

Pour la supprimer:

./VMMgr_Launcher delete MyVM [--data]

L'option --data supprime également les fichiers disques



