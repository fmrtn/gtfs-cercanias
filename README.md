# GTFS de Renfe Cercanías

El script descarga los datos publicados en formato [gtfs](https://gtfs.org/es/) de la red de Cercanías y genera un archivo por cada uno de los núcleos para su uso en [Home Assistant](https://github.com/home-assistant).

## Uso

### Linux / macOS

En la terminal:
```
chmod +x gtfs-cercanias.sh
bash gtfs-cercanias.sh
```
### Windows

En una consola de PowerShell teclea lo siguiente:

```
.\gtfs-cercanias.ps1
```

Si al ejecutar el script en Windows muestra el siguiente error:

```
+ .\script.ps1
+ ~~~~~~~~~~~~
    + CategoryInfo          : SecurityError: (:) [], PSSecurityException
    + FullyQualifiedErrorId : UnauthorizedAccess
```

Debes ejecutar el siguiente comando en un consola de PowerShell y validar con S o Y.


```
Set-ExecutionPolicy -Scope CurrentUser Unrestricted
```

Puedes verificar los archivos generados descargando la utilidad [gtfs-validator](https://github.com/MobilityData/gtfs-validator/releases) o utilizarla en línea https://gtfs-validator.mobilitydata.org/

## TODO

- [ ] filtrar stops.txt  
- [ ] filtrar calendar.txt  
- [ ] corregir warnings  
- [ ] verificar con [gtfs-validator](https://github.com/MobilityData/gtfs-validator)

## Enlaces

https://data.renfe.com/dataset/horarios-cercanias
https://gtfs.studio/
https://gtfs-validator.mobilitydata.org/
https://gtfs.org/
