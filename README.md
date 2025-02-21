# Checkpoint2

## Exercice 1

IP serveur en Nat: 10.0.2.2
(Car host only non fonctionnel)

### Q1.1 Pourquoi le ping avec les adresses IP des machines ne fonctionnent pas ?
#### Modifie la configuration sur le client pour que cela soit possible.
#### Explique ce que tu as fait et montre le par des copies d'écran.
On doit avoir la copie d'écran d'un ping fonctionnel.
![capturePing](https://github.com/user-attachments/assets/e7b6722b-9db8-43fa-9dfe-1568ca4dae5f)

### Q.1.2 Le ping avec le nom des machines ne fonctionne pas.
#### Modifie la configuration sur le client et/ou le serveur pour que cela soit possible et qu'un ping entre les 2 machines fonctionne avec le nom.
#### Explique ce que tu as fait et montre le par des copies d'écran.
Modification addresse ip fixe pour le serveur
#### Modification du réseau pour que la machine client soit dans le même réseau que le serveur
On doit avoir la copie d'écran d'un ping fonctionnel.
![capturePing](https://github.com/user-attachments/assets/9c37a890-11d4-4331-b010-f9f43858de04)


### Q.1.3 Modifie la configuration réseau du client pour qu'il soit en DHCP.
#### Vérifie le paramétrage DHCP sur le serveur et compare le avec l'adresse IP du client.
#### Explique pourquoi le client ne récupère pas la 1ère adresse disponible sur la plage DHCP du serveur ?
#### Fais une copie d'écran montrant l'adresse IP prise par le client.
![configIPClient](https://github.com/user-attachments/assets/075a6d42-8299-41a9-ab26-2f5ff5e79f45)


### Q.1.4 Est-ce que ce client peut avoir l'adresse IP 10.0.2.15 en DHCP ?
#### Si oui fais les manipulations nécessaires.
#### Explique ce que tu as fait et montre par une copie d'écran le résultat de la commande ipconfig /all sur le client.
Le serveur DHCP distribut dynamique les IP machine du réseau
![image](https://github.com/user-attachments/assets/54c47b16-15b2-4555-9627-35e1b805a16c)

![image](https://github.com/user-attachments/assets/526cbced-cdb0-45b7-8de6-fa6e389ae9c4)

## Exercice 2

#### Q.2.2 Le premier utilisateur du fichier Users.csv n'est jamais pris en compte. Modifie le script pour que cela soit le cas.

#### Q.2.3 Le champs Descriptionest importé du fichier mais non-utilisé. Modifie le code pour que ce champs soit utilisé dans la création des utilisateurs.

#### Q.2.4 Dans l'importation des utilisateurs du fichier CSV, tous les champs sont pris. Or il n'y en a qu'une partie qui est utilisé par la suite. Corrige pour qu'il n'y ait que les champs utilisés pour la création des utilisateurs qui soient importés du fichier CSV.

#### Q.2.5 Le mot de passe crée n'est pas affiché, donc on ne le connait pas. Affiche le avec le message indiquant qu'un compte est crée.

#### Q.2.6 Une fonction de création de log, nommée Log existe. Utilise là pour journaliser l'activité du script et les actions importantes du script.

#### Q.2.7 Si l'utilisateur à créer existe déjà, il n'est pas crée. Or cette information n'est pas affichée, donc on ne le sait pas. Modifie le code pour que cela s'affiche.

#### Q.2.8 L'ajout des utilisateurs dans le groupe des utilisateurs locaux ne fonctionne pas. Corrige le script pour que cela fonctionne.

#### Q.2.9 Plusieurs fois dans le code du scrip, la chaine "$Prenom.$Nom" est utilisée. Remplace cette chaîne par une variable $Name que tu initialise correctement.

#### Q.2.10 Les comptes utilisateurs créer ont un mot de passe qui expire. Corrige cela pour qu'il n'expire pas.

#### Q.2.11 Modifie le code pour que le mot de passe soit constitué de 10 caractères au lieu de 6.

### Exercice 3

###c. Etude théorique

#### Q.3.1 Quel est le matériel réseau A ?
Le maytériel du réseau A est un switch
#### Quel est son rôle sur ce schéma vis-à-vis des ordinateurs ?
Ce switch est relié par plusieurs pc qui sont dans des vlans différent, le switch sert à faire communiquer les machines entre elles

#### Q.3.2 Quel est le matériel réseau B ?
C'est un routeur
#### Quel est son rôle pour le réseau 10.10.0.0/16 ?
Elle sert de routage pour communiquer avec d'autres routeur

#### Q.3.3 Que signifie f0/0 et g1/0 sur l’élément B ?
Le f0/0 sert de liaisons avec le switch
Le g1/0 sert de liaisons avec d'autres routeur routeur
#### Q.3.4 Pour l'ordinateur PC2, que représente /16 dans son adresse IP ?
C'est le CIDR du masque de sous réseau

#### Q.3.5 Pour ce même ordinateur, que représente l'adresse 10.10.255.254 ?
c'est la passerelle réseau

#### Q.3.6 Pour les ordinateur PC1, PC2, et PC5 donne :

##### L'adresse de réseau
PC1 et PC5: 10.10.4.0
PC5: 10.11.80.0

##### La première adresse disponible
10.10.4.1
La dernière adresse disponible
L'adresse de diffusion

#### Q.3.7 En t'aidant des informations que tu as fourni à la question 3.6, et à l'aide de tes connaissances, indique parmi tous les ordinateurs du schéma, lesquels vont pouvoir communiquer entre-eux.
Toutes

#### Q.3.8 De même, indique ceux qui vont pouvoir atteindre le réseau 172.16.5.0/24.
Toutes

#### Q.3.9 Quel incidence y-a-t'il pour les ordinateurs PC2 et PC3 si on interverti leur ports de connexion sur le matériel A ?
elles ne pourront plus communique entre elles

#### Q.3.10 On souhaite mettre la configuration IP des ordinateurs en dynamique. Quelles sont les modifications possible ?
Il faufrait ajouter un server dhcp, ou configurer un router en dhcp

### d. Analyse de trames
#### Fichier 1 :

#### Q.3.11 Sur le paquet N°5, quelle est l'adresse mac du matériel qui initialise la communication ? Déduis-en le nom du matériel.
Pas de paquet 5
![image](https://github.com/user-attachments/assets/5660d9b9-0a72-49a6-897e-a11dc7ae5fa8)


#### Q.3.12 Est-ce que la communication enregistrée dans cette capture a réussi ? Si oui, indique entre quels matériel, si non indique pourquoi cela n'a pas fonctionné.

#### Q.3.13 Dans cette capture, à quel matériel correspond le request et le reply ? Donne le nom, l'adresse IP, et l'adresse mac de chaque materiel.

#### Q.3.14 Dans le paquet N°2, quel est le protocole encapsulé ? Quel est son rôle ?
ARP

#### Q.3.15 Quels ont été les rôles des matériels A et B dans cette communication ?
