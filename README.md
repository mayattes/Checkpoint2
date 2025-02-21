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
