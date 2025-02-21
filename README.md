# Checkpoint2

## Exercice 1

### Q1.1 Pourquoi le ping avec les adresses IP des machines ne fonctionnent pas ?
#### Modifie la configuration sur le client pour que cela soit possible.
#### Explique ce que tu as fait et montre le par des copies d'écran.
[! [capture ping()]
On doit avoir la copie d'écran d'un ping fonctionnel.


## 1.Donne une ligne de commande bash qui permet delister la liste des utilisateurs d'un système Linux
cmd: ls -l /etc/passwd


## 2.Quelle commande bash permet de changer les droits du fichier myfile en rwxr—r-- ?
cmd: chmod 744 "nom du fichier"

## 3.Quelle est la différence entre une variable d'environnement et une variable locale dans un script Bash, et comment pouvez-vous les définir et les utiliser ?
- Les variables d'environnements sont des variables du système accessibles à tous les programmes
- une variable locale est une variable qui ne peut être utilisée que dans la fonction ou le bloc où elle est définie


## 4.Expliquez comment fonctionne la structure de contrôle "if" dans Bash. Donnez un exemple concret de son utilisation pour prendre une décision basée sur une condition dans un script Bash.


## 5.Donne la(les) ligne(s) de commande(s) bash pour afficher le texte suivant :

## 6.Quelle commande te permet de mettre en avant le processus gedit? 
cmd: ps aux | grep gedit

## 7.Quels matériels réseaux sont sur la couche 2 et la couche 3 du modèle OSI ? Donne leurs spécificités.
les matériels réseaux de la couche 2 et 3 du modèle OSI sont les routeurs, switch, qui gère la liaisons au réseau (Ethernet > ip) des machines

## 8.Quels sont les équivalent PowerShell des commandes bash 
|  Commande linux  | Commande PowerShell     |
|:---------------|------------:|
**cp**  | Copy-Item  |
**cd** | Set-Location  |
**mkdir**  | mkdir  |
**list**  | Get-ChildItem  |

## 9.Dans la trame ethernet, qu'est-ce que le payload ?
La charge utile est un champ de longueur variable. Sa taille minimale est régie par une exigence de transmission de trame minimale de 64 octets (octets). En tenant compte de l'en-tête et du FCS, la charge utile minimale est de 42 octets lorsqu'une balise 802.1Q est présente et de 46 octets lorsqu'elle est absente.

## 10.Pourquoi les classes IP sont remplacées par le CIDR
Avec l'expansion continue d'Internet et le nombre croissant de dispositifs en ligne, le système de classes d'adresses IP a montré ses limites, conduisant à l'adoption de nouvelles technologies comme le CIDR (Classless Inter-Domain Routing) et l'introduction de l'IPv6 pour répondre à la pénurie d'adresses IP



