#Processus pour les mises à disposition Pizza Hut

##Items restant à déterminer
- [ ] mail automatique avant chaque remplissage
- [ ] message sur la GSheet une fois que les slots ont été uploadés
- [ ] automatisation envoi drivers à Roshahni pour M. Gonnet

##Questions opérationnelles
* procédure de non remplissage
    - usage du dashboard
* procédure d'absence non prévenue
    - usage du dashboard

##Building blocks
###Process pour le restaurant
* Tous les vendredi, avant 13h, le restaurant remplit la feuille du vendredi avec le nombre de coursiers souhaité
* Tous les mercredis, avant 13h, le restaurant remplit la feuille du mercredi pour les vendredi, samedi et dimanche de fin de semaine

###Blocs à remplir 
- [x] Lecture du planning + création des shifts
- [x] Update de la shift list avec update des coursiers
- [x] Mise à jour des shifts fin de semaine sur base de l'onglet du mercredi
- [ ] Upload Opé Spé

###Process to be ran periodically
* Run every friday @2PM the script PH_shifts_creation.py
* Run every day @11AM, @5PM and @9PM the script update_drivers.py
* Run every monday morning the script for payment upload to Opé Spé
* Run every wednesday @2PM the script update_shifts.py
