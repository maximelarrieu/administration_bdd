# TP9

En reprenant le [docker-compose](docker-compose.yaml) du TP précédent, on doit rajouter le service grafana auquel on connectera notre Prometheus et MySQL (mariadb).

Une fois les containers lancés : `docker-compose up -d`

On peut se rendre à l'url `localhost:3000` et arriver sur la page Grafana sur laquelle on se connecte avec `admin` et `admin` comme identifiants.

Avant de commencer il faut ajouter nos datasources ([formulaire prometheus](screenshots/prometheus_datasource.png) / [formulaire mysql](screenshots/mysql_datasource.png))

Tout est prêt pour récupérer les données !

## Premier dashboard

Rendu du premier dashboard :

![First Dashboard](screenshots/first_dashboard.png "Premier Dashboard")

Chaque panel dispose de sa metric. Dans l'édition de chacun, on retrouvera la metric des READS
<img src="screenshots/read_metric.png" width="400" height="200"/>

la metric des erreurs de connexions
<img src="screenshots/errors_metric.png" width="400" height="200"/>

ainsi que la metric du temps d'exportation
<img src="screenshots/export_metric.png" width="400" height="200"/>

## Second dashboard

Rendu du second dashboard :

![Second Dashboard](screenshots/second_dashboard.png "Deuxième Dashboard")

Comme précédemment, chaque panel dispose eux, de leur propre requête SQL.