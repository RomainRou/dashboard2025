Nouveau Dashboard 2025, dans le même esprit room card que le précèdent en essayant que les cartes soit le plus adaptable possible à chacun. Passage des cartes principale en section, suppression totale de l'addon card_mod des cartes principal pour une rapidité accrue de l'affichage, cartes plus interactives avec plus d'options, la réduction de la taille des cartes permet de moins naviguer, installation complète encore plus simple.<br>
Les chip card light,alarme,camera sur les cartes principales sont actionnable pour ne pas avoir à ouvrir le popup pour éteindre les lumières, désarmer l'alarme ou voir la vue des cameras<br>
Se sont les grandes lignes et les grandes différences entre les précédents dashboard et celui là,d'autres améliorations/modifications arriverons par la suite<br>
Si vous rencontrez des problèmes, des bugs ou avez des idées d'amélioration ne pas hésiter à m'en parler.
dashboard et popup pc<br>
<img src="https://github.com/RomainRou/dashboard2025/blob/main/dashboard%201.png" alt="Description" width="400"/>
<img src="https://github.com/RomainRou/dashboard2025/blob/main/dashboard%202.png" alt="Description" width="400"/>
<img src="https://github.com/RomainRou/dashboard2025/blob/main/dashboard%203.png" alt="Description" width="400"/>
<img src="https://github.com/RomainRou/dashboard2025/blob/main/dashboard%204.png" alt="Description" width="400"/><br><br>
dashboard et popup telephone<br>
<img src="https://github.com/RomainRou/dashboard2025/blob/main/dashboard%20tel%201.jpeg" alt="Description" width="150"/>
<img src="https://github.com/RomainRou/dashboard2025/blob/main/popup%20tel.jpeg" alt="Description" width="150"/><br>
Atention screen pris avant update 1 certaines choses ont pu changer visuellement depuis<br><br>
Addon: 
  - lovelace-meteofrance-weather-card ( https://github.com/hacf-fr/lovelace-meteofrance-weather-card ) #popup meteo
  - tabbed card (uniquement si pronote est utiliser)( https://github.com/kinghat/tabbed-card ) #tableau pronote
  - mushroom ( https://github.com/piitaya/lovelace-mushroom ) #theme general
  - card-mod ( https://github.com/thomasloven/lovelace-card-mod ) #seulement pour les popup ( en cours de suppression total)
  - bubble-card ( https://github.com/Clooos/Bubble-Card ) #pour les popup
  - <s>mini-graph-card ( https://github.com/kalkih/mini-graph-card )</s> #graph dans les popup (plus utiliser depuis update 8)
  - decluttering card ( https://github.com/custom-cards/decluttering-card ) #pour le template des cartes
  - <s>fold-entity-row ( https://github.com/thomasloven/lovelace-fold-entity-row )</s> #menu dans les popup (plus utiliser depuis update 8)
  - button-card ( https://github.com/custom-cards/button-card ) #carte principale
  - custom-icon (https://github.com/Mariusthvdb/custom-icons) #icon dynamique volets
  - pronote-card (https://github.com/delphiki/lovelace-pronote) #carte pronote, elles ne sont pas entierement changer en attente de dispo aupres du dev
  - simple thermostat (https://github.com/nervetattoo/simple-thermostat) #carte pour les thermostat
  - frigate-card (https://github.com/dermotduffy/frigate-hass-card/) #carte camera<br><br>
Integrations :
  - meteo france (pour afficher la meteo)
  - alarmo (si utiliser sinon peut etre supprimer)( https://github.com/nielsfaber/alarmo )
  - pronote (si utiliser sinon peut être supprimer)( https://github.com/delphiki/hass-pronote )
  - ainsi que les intégrations pour vos périf bien entendue et ceux que vous voulez mettre dans les cartes<br><br>
Pour les updates il vous suffit de remplacer l'ancien code lovelace.ui par le nouveau.<br><br>
Update 1 : Le changement de couleur des icons se fait dans les cartes principales a l'aide des variables:<br>
pour les entitées sur la droite de la carte:<br>
  - entity_1_icon_color_top_right<br>
  - entity_2_icon_color_top_right<br>
  - entity_3_icon_color_top_right<br><br>
pour les lumières sur la droite de la carte:<br>
  - light_1_icon_color_top_right<br>
  - light_2_icon_color_top_right<br>
  - light_3_icon_color_top_right<br><br>
pour l'entitée sur la gauche de la carte:<br>
  - entity_3_icon_color_top_left<br><br>
pour l'icone des volet sur la gauche:<br>
  - entity_cover_icon_color<br><br>
Update 2 : affichage de la temperature des pieces directement sur la room card reseigner par la ligne: - sensor_temp dans les cartes <br>
Update 3 : suppression de card_mod de la carte de commande de volet avec modification 100% = ouvert, 0% = fermé<br>
Update 4 : modification complète de la carte volets suppression de card mod et mushroom card tout en gardant le style mushroom et garant les fonctions deja présentent<br>
Update 5 : suppression et remplacement des carte custom:mushroom-entity-card par template_entity_card (pour toutes entités du bleu par defaut de ha pour on et grise pour off) et template_opening_card (pour les capteurs d'ouverture ou autre icon verte pour fermé et rouge pour ouvert) , custom:mushroom-alarm-control-panel-card par template_alarm_card dans les popup afin de continuer la suppression de card mod<br>
Update 6 : ajout de la temperature et du taux d'humidité de la pièce sur la carte du dashboard renseignable dans les cartes par les variables: - temp: et - humidity: ,si vous avez des thermostat la temperature est cliquable et renvoie vers un popup qui affiche le thermostatde la piece<br>
Update 7 : fusion de la room card et de la weather card afin de n'avoir qu'une seul carte mais regroupant les fonctions des 2 cartes , ajustement de la tailles des backgrounds<br>
Update 8 : suppresion des cartes mini graph en raison d'un probleme avec card mod , les infos qui se travais dans la carte se retrouve sur la carte du dashboard et dans la carte entity a renseigner avec la variable - sensor_power: si vous souhaiter avoir l'information de consommation et suppression des cartes fold entity row de la systeme<br>
Update 9 : quelques modifications mineure optimisation et nettoyage du code<br>
Update 10 : modification de certains nom d'entitées nettoyage du code et optimisation:<br>
pour les group prises:<br>
  - group_prises<br><br>
pour les group light:<br>
  - group_light<br><br>
pour les group volets:
  - cover_group<br>
  - entity_cover<br><br>
pour les entitées sur la droite de la carte:<br>
  - entity_1_right<br>
  - entity_2_right<br>
  - entity_2_right<br>
  - entity_1_icon_color_top_right -> entity_1_icon_color_right<br>
  - entity_2_icon_color_top_right -> entity_2_icon_color_right<br>
  - entity_3_icon_color_top_right -> entity_3_icon_color_right<br><br>
pour les entitées sur la gauche de la carte:<br>
  - entity_1_left<br>
  - entity_2_left<br>
  - entity_2_left<br>
  - entity_1_icon_color_top_left -> entity_1_icon_color_right<br>
  - entity_2_icon_color_top_left -> entity_2_icon_color_right<br>
  - entity_3_icon_color_top_left -> entity_3_icon_color_right<br><br>
pour les lumières sur la droite de la carte:<br>
  - light_1_icon_color_top_right -> light_1_icon_color_left<br>
  - light_2_icon_color_top_right -> light_2_icon_color_left<br>
  - light_3_icon_color_top_right -> light_3_icon_color_left<br><br>
pour l'icone des volet sur la gauche:<br>
  - entity_cover_icon_color<br><br>
pour l'alarme:<br>
  - entity_alarme<br>
  - code_alarm<br><br>
pour la boite aux lettres:<br>
  - capteur_bal<br><br>
Update 11 : résolution d'un bug pour le chip caméra , maintenant il s'affiche une fois l'alarme armée en mode absent et nuit<br>
Update 12 : resolution de quelques bugs sur la chip card camera s'affiche avec alarmo activé en mode nuit/absent la couleur peut etre changer dans les variables de la carte, la chip alarme reste aficher quand alarmo passe a triggered (declenchée), l'icone camera passe en rouge quand alarmo est declenchée<br>
Update 13: modification de la carte de gestion de radiateur electrique avec module zigbee mini-z1-2ch modifier avec 2 diodes , mise en place d'un blueprint pour la gestion du chauffage avec extinction a l'ouverture de la fenetre et remis en place du cycle a la fermeture avec des input_select pour la selection du mode et des input_text pour la sauvegarde du mode avant ouverture de la fenetre , modification de certaines fonctions et de visuel divers<br>
Update 14: modification de la carte chauffage<br><br>
Update en cour suppression de card mod<br>
Instalation du dashboard:<br><br>
Dans home assistant cliquer sur le crayon pour modifier le dashboard en haut à droite<br>
<img src="https://i.gyazo.com/94495911cb00a289e33ccccaa2199985.png" alt="Description" width="200"/><br>
Ensuite il faut cliquer sur les 3 points encore en haut à droite, et appuyer sur éditeur de configuration<br>
<img src="https://i.gyazo.com/46c23e632bcfaac701cf0d0c17eaf874.png" alt="Description" width="200"/><br>
Copié l'intégralité du fichier lovelace.ui avant la ligne view<br>
<img src="https://i.gyazo.com/4cae48a22539b91cf6b774fc060d7fde.png" alt="Description" width="200"/><br>
Enregistré et quitter avec la croix en haut à gauche<br><br>
Maintenant il faut créé un nouveau dashboard en mode section<br>
<img src="https://i.gyazo.com/fed94454ef5c114f1a34f48ced428ae1.png" alt="Description" width="200"/><br>
Pour le nombre de section c'est libre à vous<br> 
<img src="https://i.gyazo.com/062ecd10c9cb40f47d510737bce57b70.png" alt="Description" width="200"/><br>
Dans le nouveau dashboard il faut ajouter une carte manuel<br>
<img src="https://i.gyazo.com/2db46db25d00724282166ece85dec922.png" alt="Description" width="200"/>
<img src="https://i.gyazo.com/31ff55443f3ba690d814bbcb1c2f0d0c.png" alt="Description" width="200"/><br>
Dans la carte manuel il faut copié la carte choisi dans le fichier dashboardcard.yaml<br>
<img src="https://i.gyazo.com/1ef4acdc994d4e721dfd5b92510ab09d.png" alt="Description" width="200"/><br>
Et refaire la manip avec une carte manuel pour les popup en prenant le popup correspondant dans le fichier popupcard.yaml<br>
Dans les cartes il vous suffit de changer les entitées,sensors etc....<br>
Des mises à jour serons faites au fur et à mesure pour avoir encore plus de flexibilité pour les cartes et de personnalisation des cartes. bonne amusement 
