# TocToc-setup


## Préparation de la carte SD

### Prérequis
Télécharger la dernière version de [Raspberry Pi Imager](https://www.raspberrypi.com/software/) pour votre ordinateur [windows](https://downloads.raspberrypi.org/imager/imager_latest.exe), [Mac](https://downloads.raspberrypi.org/imager/imager_latest.dmg) ou [Ubuntu x86](https://downloads.raspberrypi.org/imager/imager_latest_amd64.deb).

- **image** : Raspberry Pi OS Lite(32bit)
- **model** : Raspberry Pi Zero W
- une carte micro-sd de 16go minimum

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

## Une fois connecté au SSH
- 1 - `sudo apt update`
- 3 - `sudo apt install git -y`
- 2 - `cd /home/toctoc/`
- 4 - `git clone https://github.com/PGaillot/TocToc-setup.git`
- 5 - `cd TocToc-setup/`
- 6 - `sudo chmod +x setup.sh`
- 7 - `sudo ./setup.sh`
  
--- 

```` bash
sudo apt update && sudo apt install git -y && \
cd /home/toctoc/ && git clone https://github.com/PGaillot/TocToc-setup.git && \
cd TocToc-setup/ && sudo chmod +x setup.sh && sudo ./setup.sh
