# SwinGraf
Swingraf is an incredible LED panel made with an ESP32.  
It can display your messages, big clocks, audio spectrum music, animated gifs, weather, RSS feeds... 


[![SwinGraf Demo](images/SwinGraf.gif)](https://youtu.be/1jUjtwE3uyU "SwinGraf Demo")


Demo 1 : Textes, Horloges et spectre(s) audio, avec 3 panneaux SwinGraf superposés.  
https://youtu.be/1jUjtwE3uyU



IMPORTANT :
Le code et les schémas de cette réalisation seront disponibles à la rentrée 2021.  
Merci pour votre patience...


SwinGraf est un panneau LED RGB 128x32 avec connectivité WiFi
On peut le commander depuis une application Android, ou un logiciel Windows, ou un simple navigateur Internet.



SwinGraf peut afficher :

- Des textes sur plusieurs lignes. Les messages sont définissables à l'avance, un clic pour les lancer.
- Horloge(s) : Plusieurs styles d'horloges avec couleurs ou images modifiables.
- La météo de la ville de votre choix.
- Les infos RSS de votre choix (compatible avec la plupart des flux RSS ou XML disponibles).
- Le spectre audio de vos musiques : Nombreux effets prédéfinis. Connexion audio sur la sortie ligne ou par Bluetooth
- Gestion des déplacements des GIF sur l'écran.
- Upload et téléchargement d'images GIF animées en ligne.
- Upload et téléchargement de vos images personnelles et enregistrement sur la carte SD de SwinGraf.
- Dessin en live : Dessinez ce que vous voulez sur votre écran de smartphone et cliquez pour l'envoyer sur l'afficheur. 
- Chaque fonction fait partie d'une séquence qui peut tourner en boucle
- Possibilité d'activer ou désactiver, à tout moment, chaque module de la séquence.
- Mise à jour du firmware, avec recherche automatique et affichage des versions.

SwinGraf est réalisé avec un ESP32 et deux RGB LED Panel de type HUB75 64x32 (soit un total de 128x32 leds).
Le circuit imprimé comprend aussi un module audio Bluetooth 5.0 pour une connectivité de la musique sans fil.
Dans les versions à venir, je prévois une connectivité avec d'autres services (domotique, réseaux sociaux, etc.)







Tags : ESP32, HUB75, LED panel, Arduino, Audio spectrum, music visualiser, GIF animated, text marquee, big clock, weather 




Liste des librairies utilisée et remerciements :


Arduino IDE
https://github.com/arduino/Arduino

Arduino ESP32
https://github.com/espressif/arduino-esp32


ESP32-HUB75-MatrixPanel-I2S-DMA
https://github.com/mrfaptastic/ESP32-HUB75-MatrixPanel-I2S-DMA


Adafruit_GFX
https://github.com/adafruit/Adafruit-GFX-Library

U8g2_for_Adafruit_GFX
https://github.com/olikraus/U8g2_for_Adafruit_GFX


ESPAsyncWebServer et AsyncWebSocket
https://github.com/me-no-dev/ESPAsyncWebServer


AnimatedGIF
https://github.com/bitbank2/AnimatedGIF

AnimatedGIF (version modifiée) :
https://github.com/MichaelBell/pico-projects/tree/master/sdgif


ArduinoJson
https://github.com/bblanchon/ArduinoJson

ezTime
https://github.com/ropg/ezTime

CircularBuffer
https://github.com/rlogiacco/CircularBuffer


elapsedMillis
https://github.com/pfeerick/elapsedMillis



Autres services ou applications :

Les données météo sont fournies par openweathermap. Il suffit d'ouvrir un compte pour obtenir une clé API.
https://openweathermap.org/

Les Flux RSS sont gérés par un serveur PHP personnel avec un agrégateur de Flux.
Ce même serveur dispose d'un espace FTP permettant l'upload et le téléchargement d'images GIF, et les mises à jour du firmware. 
Si vous ne disposez pas d'un serveur, il est possible d'enregistrer les images sur la carte SD de SwingGraf avant de les afficher.


Schémas, circuit Imprimé
Information à compléter ...


Boitier et fichier 3D
Il sera possible de télécharger les fichiers STL (Print 3D) pour imprimer les éléments de construction du boitier.





Sources d'inspiration :

MD Parola
https://github.com/MajicDesigns/MD_Parola
J'avais réalisé un petit afficheur (rouge) avec des MAX7219 et MD_Parola. Les effets de cette librairie étaient très réussis.  
Je n'ai pas été en mesure de convertir cette librairie pour les panneaux RGB HUB75, mais Adafruit_GFX m'a permis de créer quelques effets de textes similaire


