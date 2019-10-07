# TP 3 & 4 d'Architectures Distribuées
A l'aide d'une extension Chrome Advanced Rest Client : l'ajout de l'adresse du service Paas associé à la requête choisie du scénario permet d'obtenir les informations demandées. 
Par exemple : 

Pour obtenir la liste des animaux 
on entre l'adresse suivante dans l'url de l'application chrome Advanced Rest Client : 
http://rest-service-rested-quokka.eu-gb.mybluemix.net/zoo-manager/animals 
On selectionne ensuite la methode GET 
Puis on insère les données  {"name":"nouveau_nom","cage":"usa","species":"chipmunk"} 
Enfin on clique sur SEND pour obtenir les informations

Pour PUT
on entre l'adresse suivante dans l'url de l'application chrome Advanced Rest Client : 
http://rest-service-rested-quokka.eu-gb.mybluemix.net/zoo-manager/animals 
On selectionne ensuite la methode PUT 
Puis on insère les données suivante par exemple 
Payload : {"name":"nouveau_nom","cage":"usa","species":"chipmunk"} 
Enfin on envoie les informations précedentes en cliquant sur SEND


Idem pour la suppression de tous les animaux : 
http://rest-service-rested-quokka.eu-gb.mybluemix.net/zoo-manager/animals 
En selectionnant la methode delete


Pour la creation d'un animal, depuis l'application AdvancedRestClient avec les informations suivantes : 
http://rest-service-rested-quokka.eu-gb.mybluemix.net/zoo-manager/animals/<nouveau_id_animal> 
Puis la methode : post 
Puis : Payload : {"name":"nouveau_nom","cage":"usa","species":"nouvelle_espèce"} 
Enfin : Content-Type : application/json


Idem pour la modification d'un animal existant 
http://rest-service-rested-quokka.eu-gb.mybluemix.net/zoo-manager/animals/<id_animal_modifié> 
Avec la methode : PUT
Puis : Payload : {"name":"nouveau_nom","cage":"usa","species":"nouvelle_espèce"} 
Enfin : Content-Type : application/json


Pour la suppresion d'un animal par son id :
http://rest-service-rested-quokka.eu-gb.mybluemix.net/zoo-manager/animals/<id_animal_a_supprimé> 
Avec la méthode : delete


Pour afficher les animaux par leurs noms on aurais lancé une requette get directement depuis le navigateur
Par exemple : 
http://rest-service-rested-quokka.eu-gb.mybluemix.net/zoo-manager/find/byName/Canine


Pour afficher un annimal par sa position on aurais lancé la requette get directement depuis sur le navigateur 
Par exemple : 
http://rest-service-rested-quokka.eu-gb.mybluemix.net/zoo-manager/find/at/49.305&1.2157357


Pour afficher des animaux par leurs position on aurais lancé la requette get directement depuis sur le navigateur 
Par exemple :
http://rest-service-rested-quokka.eu-gb.mybluemix.net/zoo-manager/find/near/49.305&1.2157357


Enfin pour suppresion d'un animal avec son emplacement, on utiliserais l'extension ARC avec :
http://rest-service-rested-quokka.eu-gb.mybluemix.net/zoo-manager/animals/at/ 
Puis la méthode : delete


