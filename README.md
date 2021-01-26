# Docker Image - Esquite Framework

## v0.2
- [ES] Todos los componentes de Esquite en un container único
- [EN] Esquite All-in-one container 

- [ES] El script de inicialización soporta opciones en varias lenguas :)
- [EN] Startup script with multi-language support (English|Spanish|Nahuatl*) for startup options

- [ES] Se regeneró la imagen Docker que es mas pequeña (basada en Linux Alpine)
- [EN] Smaller Docker image (Linux Alpine based)

### Usage | Uso:

## Quick Start | Inicio Rápido

```
git clone https://github.com/ElotlMX/Esquite-docker.git
./esquite-docker.sh start
```
- [EN] And browse http://localhost  (Default corpus-admin password is `elotl`. To change it please set the variable `CFG_CORPUS_ADMIN_PASS=elotl` on file `docker-compose.yml`)
- [ES] Navegar en http://localhost  (El password default de corpus-admin es `elotl`. Para cambiarlo hay que definit la variable `CFG_CORPUS_ADMIN_PASS=elotl` en el archivo `docker-compose.yml`

## Options | Opciones
```
./esquite-docker.sh 

##############################################
 Esquite Docker script   - Comunidad ElotlMX
----------------------------------------------
 Github: https:///github.com/elotlmx
 Web   : Elotl.mx
##############################################


[EN ] ERROR: Unknown Option: Syntax:    ./esquite-docker (start|stop|restart|destroy|info|update|recreate)
[ES ] ERROR: Opción no valida. Sintaxis:    ./esquite-docker (iniciar|detener|reiniciar|destruir|info|actualizar|recrear)
[NAH] TLATLACOLLI: Opción no valida. Sintaxis:    ./esquite-docker (pehualtia|cahua|re-pehualtia|tlapoloa|tlanonotzaliztli|yancuic|tlaana)

```

## Docker-compose options | Opciones de Docker compose

### Opciones Generales | General Options
- [ES] El archivo de configuración de `docker-compose.yml` se puede personaizar para las opciones generales de Esquite
- [EN] The configuration file for `docker-compose.yml` can be customized with the basic option of Esquite

### Índice externo de Elasticsearch | External Elasticsearch Index
- [ES] Si se desea usar un indice externo de Elasticseach, solo se deben cambiar las variables `CFG_URL` y `CFG_INDEX`. Si estas opciones no se modifican, se creará un índice automáticamente en un container generado por el script de inicialización
- [EN] If an external Elasticsearch index needs to be used, you only need to set the two options `CFG_URL` and `CFG_INDEX`. If these options are not set, then a new index will be created running in a container generated by the startup script

### Actualización de versión de Esquite | Esquite version Updates
- [ES] Se puede habilitar la actualización de Esquite cada vez que se reincie el container activando la opción `CFG_UPDATE_ON_BOOT` o manualmente por medio de las opociones `update` o `actualizar` o `tlanonotzaliztli` con el script `./esquite-docker.sh`
- [EN] It is possible to enable automatic update on each container restart by enabling the option `CFG_UPDATE_ON_BOOT` or manually by using any of the options `update` or `actualizar` or `tlanonotzaliztli` with the startup script `./esquite-docker.sh` 
