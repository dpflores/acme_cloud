# Levantamiento del servicio de Thingsboard

En la carpeta del repositorio primero crear y dar acceso a las siguientes carpetas

``` 
mkdir -p ./data/mytb-data && sudo chown -R 799:799 ./data/mytb-data
mkdir -p ./data/mytb-logs && sudo chown -R 799:799 ./data/mytb-logs
```

Luego correr 

```
docker compose up
```
