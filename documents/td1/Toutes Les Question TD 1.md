***[LES QUESTION CLIQUE FORT !!!](https://slamwiki2.kobject.net/_media/sio/1_-_architecture_web.pdf)***

   

***Question 1***
_____________________________________________________________________________________________________________________________    

**Méthode Get**

La méthode HTTP GET demande une représentation de la ressource spécifiée. Les requêtes GET doivent uniquement être utilisées afin de récupérer des données. Elle est Sûre, idempotente et peux être mise en cache mais elle ne peux pas recevoir la requête a un corps


**Méthode POST**

La méthode HTTP POST envoie des données au serveur souvent envoyée secrètement via un formulaire HTML et a pour résultat un changement sur le serveur en contre partie elle n'est pas sûre et idempotente et peux etre mise en cache si seulement une info de péremption est incluse 


***Question 2***
_____________________________________________________________________________________________________________________________    

| Information      | ***HTTP Get***  |***HTTP Post***|
| :---        |    :----:   |          ---: |
| Visibilité    | Visible pour l’utilisateur dans le champ d’adresse     | Invisible pour l’utilisateur  |
| Marque-page et historique de navigation | Les paramètres de l’URL sont stockés en même temps que l’URL.	        | L’URL est enregistrée sans paramètres URL.      |
|  Cache et fichier log du serveur| Les paramètres de l’URL sont stockés sans chiffrement	         | Les paramètres de l’URL ne sont pas enregistrés automatiquement.      |
| Comportement lors de l’actualisation du navigateur / Bouton « précédent »  | Les paramètres de l’URL ne sont pas envoyés à nouveau.	          | Le navigateur avertit que les données du formulaire doivent être renvoyées.    |
| Type de données  | Caractères ASCII uniquement.	           | 	Caractères ASCII mais également données binaires.	      |
| Longueur des données	   | Limitée - longueur maximale de l’URL à 2 048 caractères.	          | Illimitée.   |


***Question 3***
_____________________________________________________________________________________________________________________________    

**Le Protocole HTTP est extensible**

À partir de HTTP/1.0, les en-têtes HTTP permettent d'étendre facilement le protocole et de mener des expérimentations avec celui-ci. De nouvelles fonctionnalités peuvent même être introduites par un simple accord entre le client et le serveur à propos de la sémantique des nouveaux en-têtes.

L’ensemble des règles permettant de transférer des fichiers tels que du texte, des images, du son, de la vidéo et d’autres fichiers multimédias sur le Web. Dès qu’un utilisateur ouvre son navigateur Web, il utilise indirectement le protocole HTTP


***Question 4***
_____________________________________________________________________________________________________________________________    

HTTP est considéré comme un protocole sans état car chaque commande est exécutée indépendamment, sans aucune connaissance des commandes qui la précèdent . C'est la principale raison pour laquelle il est difficile de mettre en œuvre des sites Web qui réagissent intelligemment aux entrées des utilisateurs.

L'utilisation d'un protocole sans état dans un logiciel serveur permet de simplifier son design, car on se libère de toute la gestion compliquée de l'espace mémoire requis pour enregistrer l'état des échanges en cours. Si une session cliente meurt à mi-transaction, aucune partie du système n'est tenue de procéder au nettoyage de l'état en cours du serveur. Un inconvénient majeur du design stateless réside dans la nécessité d'inclure des informations supplémentaires dans chaque requête, et ces informations supplémentaires doivent être interprétées par le serveur.

***Question 5***
_____________________________________________________________________________________________________________________________    

![Image](https://images.squarespace-cdn.com/content/v1/60f1a490a90ed8713c41c36c/1628807693445-MJX2ZG1CAYVBGG37CGUU/image-asset.png
)

***Question 6***
_____________________________________________________________________________________________________________________________    

100s : Codes d’information indiquant que la demande initiée par le navigateur se poursuit.     

200s : Les codes de réussite sont renvoyés lorsque la requête du navigateur est reçue, comprise et traitée par le serveur.       
 
300s : Codes de redirection renvoyés lorsqu’une nouvelle ressource a été substituée à la ressource demandée.           

400s : Les codes d’erreur des clients indiquant qu’il y a eu un problème avec la requête.                  

500s : Codes d’erreur du serveur indiquant que la requête a été acceptée, mais qu’une erreur sur le serveur a empêché l’exécution de la requête.          

***Question 7***
_____________________________________________________________________________________________________________________________    

![Image](https://lh6.googleusercontent.com/proxy/dkDJiEfpdi0F1zP07K-6kk4IIXmWNHmg75BfXJAGTEe11Zc3cRUCk0GH2qtnvB6wmz13NIKPoMpBoNlWy-E)

Lorsqu'un client souhaite obtenir une ressource, il la demande via une URL. Le serveur utilise alors cette URL pour choisir l'une des variantes disponibles. Chaque variante est appelée une représentation. Le serveur renvoie alors une représentation donnée au client.



***Question 10***
_____________________________________________________________________________________________________________________________    


| En-Têtes      | ***Expliquer***  |***Illustrez***|
| :---        |    :----:   |          ---: |
| Accept    |  fournit au serveur la liste des types de contenu acceptables pour le client.     |![image](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcROdhT8umDzN4T6pN2X6IaCA7st9RUmfBALJQ&s)   |
| Authorization |  transmet les informations d’authentification du client au serveur.       | ![image](https://www.medianova.com/wp-content/uploads/2023/03/Authentication.jpg)     |
| Cache-Control|spécifie les directives de mise en cache à respecter par le client et le serveur.          |![image](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQomnRXZ37zsuVPU82PUqjYHyzqL2D9fl4_iA&s)      |
| Location  |  indique l’URL vers laquelle le client doit être redirigé (utilisé principalement dans les réponses de redirection).         |![image](https://ventsmagazine.com/wp-content/uploads/2022/07/1_v4Pp0pG5WMbknprejifVmw.png)   |
| Content-Type  |	ndique le type de contenu (MIME) du corps de la requête ou de la réponse.           | ![image](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQomnRXZ37zsuVPU82PUqjYHyzqL2D9fl4_iA&s)     |


