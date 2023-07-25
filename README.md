# SRV-Gitea

## Lancement du conteneur

```shell
docker-compose up --build -d
```

## Arret du conteneur

```shell
docker-compose down --remove-orphans
```

## Rentrer dans le conteneur

```shell
docker exec -it gitea bash
docker exec -it postgresql-gitea bash
```

## Informations

### Gitea

- Aucun fichier de configuration est nécessaire, Gitea permet de tout configurer depuis l'interface web.

- Les données persistantes sont dans le dossier `./gitea_data` sur l'hôte.

### Postgresql

- La seule variable d'environement utilisée est stockée dans un "secrets" dans le dossier `./.secrets/` sur l'hôte.

- Les données persistantes sont dans le dossier `./postgresql_data` sur l'hôte.
