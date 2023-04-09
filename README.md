# Gitlab

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
docker exec -it gitlab sh
```

## Informations

Toutes les données sont gérés dans des points de montage.
- .gitlab_config/
- .gitlab_logs/
- .gitlab_data/
