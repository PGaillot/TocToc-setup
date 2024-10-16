# TocToc-setup

## Préparation de la carte SD

### Prérequis
Télécharger la dernière version de [Raspberry Pi Imager](https://www.raspberrypi.com/software/) pour votre ordinateur [windows](https://downloads.raspberrypi.org/imager/imager_latest.exe), [Mac](https://downloads.raspberrypi.org/imager/imager_latest.dmg) ou [Ubuntu x86](https://downloads.raspberrypi.org/imager/imager_latest_amd64.deb).

- **image** : Raspberry Pi OS Lite(32bit).
- **model** : Raspberry Pi Zero W.
- **stockage** : une carte micro-sd de 16go minimum.
  
---

dans la fenêtre d'option choisir de modifier les réglages avec : 
#### Général
- [x] nom d'hôte : *raspizerow*.local
- [x] Définir nom d'utilisateur en mot de passe
  - Nom d'utilisateur : *toctoc*
  - Mot de passe : *Votre-mot-de-passe*
- [x] Configurer le Wi-Fi

#### Services
- [x] Activer SSH
  - [x] utiliser un mot de passe pour l'authentification.

## Trouver l'ip du raspberry
https://raspberry-pi.fr/trouver-adresse-ip-raspberry-pi/

## Se connecter en SSH
- 1 - `ssh toctoc@raspizerow.local` ou `ssh toctoc@192.168.1.XX` (*votre ip*)
- 2 - Entrez votre *mot de passe*
- 3 - `sudo apt update`
- 4 - `sudo apt install git -y`
- 5 - `cd /home/toctoc/`
- 6 - `git clone https://github.com/PGaillot/TocToc-setup.git`
- 7 - `cd TocToc-setup/`
- 8 - `sudo chmod +x setup.sh`
- 9 - `sudo ./setup.sh -i ID-DU-DEVICE -w WIFI-PASSWORD`  
  
--- 

```` bash
sudo apt update && sudo apt install git -y && \
cd /home/toctoc/ && git clone https://github.com/PGaillot/TocToc-setup.git && \
cd TocToc-setup/ && sudo chmod +x setup.sh && sudo ./setup.sh
````
--- 

### Connection
Par defaut le SSID du wifi est *TocToc-123* et le password *Toc*2=T0Ct0C!*
