Nouveau dashboard 2025, dans le même esprit que le precedent en assayant qu'il sois le plus adaptable possible a chacun. passage des cartes principale en section , supression total de l'addon card_mod des cartes principal pour une rapidité accrue de l'affichage, cartes plus interactives avec plus d'options, la reduction de la taille des cartes permet de moins naviguer , installation complete encore plus simple.<br>
Les chip card light,alarme,camera sur les cartes principal sont actionnable pour ne pas avoir a ouvrir le popup pour eteindre les lumieres, desarmer l'alarme ou voir la vue des cameras
dashboard et popup pc<br>
<img src="https://github.com/RomainRou/dashboard2025/blob/main/dashboard%201.png" alt="Description" width="400"/>
<img src="https://github.com/RomainRou/dashboard2025/blob/main/dashboard%202.png" alt="Description" width="400"/>
<img src="https://github.com/RomainRou/dashboard2025/blob/main/dashboard%203.png" alt="Description" width="400"/>
<img src="https://github.com/RomainRou/dashboard2025/blob/main/dashboard%204.png" alt="Description" width="400"/><br><br>
dashboard et popup telephone<br>
<img src="https://github.com/RomainRou/dashboard2025/blob/main/dashboard%20tel%201.jpeg" alt="Description" width="150"/>
<img src="https://github.com/RomainRou/dashboard2025/blob/main/popup%20tel.jpeg" alt="Description" width="150"/><br><br>
Addon: 
  - lovelace-meteofrance-weather-card ( https://github.com/hacf-fr/lovelace-meteofrance-weather-card ) #popup meteo
  - tabbed card (uniquement si pronote est utiliser)( https://github.com/kinghat/tabbed-card ) #tableau pronote
  - mushroom ( https://github.com/piitaya/lovelace-mushroom ) #theme general
  - card-mod ( https://github.com/thomasloven/lovelace-card-mod ) #seulement pour les popup 
  - bubble-card ( https://github.com/Clooos/Bubble-Card ) #pour les popup
  - mini-graph-card ( https://github.com/kalkih/mini-graph-card ) #graph dans les popup
  - decluttering card ( https://github.com/custom-cards/decluttering-card ) #pour le template des cartes
  - fold-entity-row ( https://github.com/thomasloven/lovelace-fold-entity-row ) #menu dans les popup
  - button-card ( https://github.com/custom-cards/button-card ) #carte principale
  - custom-icon (https://github.com/Mariusthvdb/custom-icons) #icon dynamique volets
  - pronote-card (https://github.com/delphiki/lovelace-pronote) #carte pronote, elle ne sont pas entierement changer en attente de dispo aupres du dev  
  - frigate-card (https://github.com/dermotduffy/frigate-hass-card/) #carte camera


Integrations:
  - meteo france (pour afficher la meteo)
  - alarmo (si utiliser sinon peut etre supprimer)( https://github.com/nielsfaber/alarmo )
  - pronote (si utiliser sinon peut etre supprimer)( https://github.com/delphiki/hass-pronote )
  - ainsi que les intégrations pour vos perif bien entendue et ceux que vous voulez mettre dans les cartes<br><br>
Instalation du dashboard:<br><br>
Dans home assistant cliquer sur le crayon pour modifier de le dashboard en haut a droite<br>
<img src="https://i.gyazo.com/94495911cb00a289e33ccccaa2199985.png" alt="Description" width="200"/><br>
Ensuite il faut cliquer sur les 3 points encore en haut a droite , et appuyer sur editeur de configurationw<br>
<img src="https://i.gyazo.com/46c23e632bcfaac701cf0d0c17eaf874.png" alt="Description" width="200"/><br>
Copié l'integralité du fichier lovelace.ui avant la ligne view<br>
<img src="https://i.gyazo.com/4cae48a22539b91cf6b774fc060d7fde.png" alt="Description" width="200"/><br>
Enregistré et quitter avec la croix en haut a gauche<br><br>
Maintenant il faut cré un nouveau dashboard en mode section<br>
<img src="https://i.gyazo.com/fed94454ef5c114f1a34f48ced428ae1.png" alt="Description" width="200"/><br>
Pour le nombre de section c'est libre a vous<br> 
<img src="https://i.gyazo.com/062ecd10c9cb40f47d510737bce57b70.png" alt="Description" width="200"/><br>
Dans le nouveau dashboard il faut ajouter une carte manuel<br>
<img src="https://i.gyazo.com/2db46db25d00724282166ece85dec922.png" alt="Description" width="200"/>
<img src="https://i.gyazo.com/31ff55443f3ba690d814bbcb1c2f0d0c.png" alt="Description" width="200"/><br>
Dans la carte manuel il faut copié la carte choisi dans le fichier dashboardcard.yaml<br>
<img src="https://i.gyazo.com/1ef4acdc994d4e721dfd5b92510ab09d.png" alt="Description" width="200"/><br>
et refaire la manip avec une carte manuel pour les popup en prenant le popup correspondant dans le fichier popupcard.yaml<br>
Dans les cartes il vous suffit de changer les entitées,sensors etc....<br>
des mise a jours serons faites au fur et a mesure pour avoir encore plus de flexibilité pour les cartes 
