# TocToc-setup


## Préparation de la carte SD

### Prérequis
Télécharger la dernière version de [Raspberry Pi Imager](https://www.raspberrypi.com/software/) pour votre ordinateur [windows](https://downloads.raspberrypi.org/imager/imager_latest.exe), [Mac](https://downloads.raspberrypi.org/imager/imager_latest.dmg) ou [Ubuntu x86](https://downloads.raspberrypi.org/imager/imager_latest_amd64.deb).

image : Raspberry Pi OS Lite(32bit)


## Trouver l'ip du raspberry

## Une fois connecté au SSH
- 1 - `sudo apt update`
- 3 - `sudo apt install git -y`
- 2 - `cd /home/toctoc/`
- 4 - `git clone https://github.com/PGaillot/TocToc-setup.git`
- 5 - `cd TocToc-setup/`
- 6 - `chmod +x setup.sh`
- 7 - `sudo ./setup.sh`
  
--- 

```` bash
sudo apt update && sudo apt install git -y && \
cd /home/toctoc/ && git clone https://github.com/PGaillot/TocToc-setup.git && \
cd TocToc-setup/ && sudo chmod +x setup.sh && sudo ./setup.sh
