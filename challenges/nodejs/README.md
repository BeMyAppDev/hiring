Event store
--

### Description
L’application permettra de récupérer les différents évènements javascript (conférences, meetups, workshops) à venir dans différents pays. Elle sera uniquement accessible via une API donnée et ne disposera d'aucune interface graphique.

### Features
Toutes les 24 heures, l’application vérifiera la présence de nouveaux évènements javascript à partir du site Lanyrd (http://lanyrd.com/topics/javascript/) et mettra à jour une base de données.

L’api de l’application exposera une ressource `events`. Elle sera accessible via le chemin `/api/events` et respectera les conventions REST:

- `GET /api/events`: Renvoie la liste de tous les prochains évènements disponibles
- `POST /api/events` --> Créer un nouvel évènement à partir des données passées dans le corps de la requête
- `GET /api/events/:id` --> Renvoie l'évènement correspondant à l’identifiant donné en paramètre
- `PUT /api/events/:id` --> Met à jour l'évènement correspondant à l’identifiant donné en paramètre, avec les données passées dans le corps de la requête
- `DELETE /api/events/:id` --> Supprime l'évènement correspondant à l’identifiant donné en paramètre

### Contraintes
- L'application devra être implémentée avec Node.js (choix libre pour d'éventuelles librairies et/ou frameworks à utiliser)
- Le JSON sera utilisé pour converser avec l'api
- Github sera utilisé pour la réalisation du projet
- Une documentation sera fournie pour installer l'application et la lancer



