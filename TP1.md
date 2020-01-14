# Installation serveurs

## Installation d'une nouvelle machine
Suivre le tuto à ce [lien](www.ipgp.fr/~lecocq), suivre le TP 1.

## Post-installation

### 1. Installation de SSH

Installer ssh
> apt-get install ssh

Configurer ssh : 

- autoriser les connexions distantes avec mot de passe
> nano /etc/ssh/sshd_config

- décommenter la ligne :
> PermitRootLogin yes

- et la ligne
> PasswordAuthentification

- mettre la carte réseau de la machine en bridge

### 2. Pour aller plus loin

> preseed permet d'installer automatiquement une Debian en listant dans un fichier tous les paramètres voulus.

- Récupération du password root

~~~    redémarrer la machine en restant appuyé sur la touche ESC
    choisir le boot de type "Recovery Mode"
    Dans le shell :
    taper la commande "passwd votre_nom_d_utilisateur"
    entrer le nouveau mot de passe
    redémarrer la machine
~~~

