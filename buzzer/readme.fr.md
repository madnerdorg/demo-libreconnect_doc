
[English](index.html)

[![Libre Connect](https://madnerdorg.github.io/libreconnect/doc/img/libreconnect_devices_banner.png)](https://madnerdorg.github.io/libreconnect/doc/fr/devices)   
[Télécharger Buzzer](https://github.com/madnerdorg/buzzer/archive/master.zip) / [Application](http://madnerd.org/interface/midi)     /   [LibreConnect](https://madnerdorg.github.io/libreconnect/) / [Source](https://github.com/madnerdorg/buzzer) 

![Midi Buzzer](doc/buzzer_photo.jpg)  
Jouer de la musique / créer une alarme avec un buzzer.

- [Applications](#applications)
- [Commandes](#commandes)
- [Construire buzzer](#construire-buzzer)
- [Impression 3D](#impression-3d)

# Applications

## Clavier MIDI
![Midi Buzzer](doc/buzzer_photo2.jpg)  
* Brancher votre **clavier MIDI**.
* Aller sur [http://madnerd.org/interface/midi](http://madnerd.org/interface/midi)

## Logiciel Midi
![buzzer on LMMS](doc/buzzer_lmms.png)
Vous pouvez aussi composer des musiques qui seront jouées par le buzzer.   

### LoopMidi
![LoopMidi Add Midi Port](doc/loopMidi.png)     
Nous allons utiliser loopMidi pour générer des ports midi virtuels sur Windows.
* Télécharger: [loopmidi](http://www.tobias-erichsen.de/software/loopmidi.html)   
* Cliquez sur **+** pour créer un port midi virtuel

### LMMS
Des exemples sont disponibles dans **lmms/**

![buzzer on LMMS](https://github.com/madnerdorg/buzzer/raw/master/doc/buzzer_lmms.png)
* Télécharger **LMMS** : https://lmms.io/download/#windows
* Sur **TripleOscillator** mettez le volume à 0
* Cliquer sur la roue près de **TripleOscillator**
* Cliquer sur Midi et choisissez votre **port midi virtuel** (**par défaut: Loopmidi**)

# Commandes
* /info --------> affiche le nom:port    
* X -------> Où x est la fréquence en HZ.
* OFF -------> Arrête le son    

# Construire buzzer

## Composants
* Arduino nano CH340G: 2€    
* 10 Buzzer : 1.80€  (1 Buzzer:0.18€)  
* Resistor pack 400pcs (3€) (1 resistor: 0.0071€) 
* 5 pcs stripboard (1.18€) (1 stripboard : 0.24€ )  
* Total : 7.98€ (2.43€)   

## Branchement
N'oubliez pas d'isoler le circuit de l'Arduino  
### Buzzer seul
![UBuzzer Wiring](doc/buzzer_wiring.png)   
* Pin 9 : RÉSISTANCE (100Ω) --- Buzzer +   
* Pin 10 : Buzzer -    

### Buzzer/Led
Vous pouvez ajouter une LED (**avant la résistance**)
* Pin 9 : RESISTANCE (100Ω) --- Led + / Buzzer +   
* Pin 10 : LED - / Buzzer -    

## Impression 3D
Ce modèle est un **boitier réutilisable** pour des projets avec un arduino nano    
Modèles fait par Olivier Sarrailh : [https://github.com/madnerdorg/buzzer/tree/master/3D]()

> Le boitier peut être légèrement trop petit pour être correctement fermé

# Licences
## Buzzer.ino
* Auteur: Rémi Sarrailh (madnerd.org)   
* Licence: MIT

## ToneAC
* Author: Tim Eckel
* Licence : GNU GPL v3
* Lien: https://bitbucket.org/teckel12/arduino-toneac/wiki/Home
* Donation : [PayPal](https://bitbucket.org/teckel12/arduino-toneac/wiki/Home#!show-your-appreciation)

