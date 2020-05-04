# Elastic & CIU

Demos para la sesión del Stack Elastic y Machine Learning para la Universidad Internacional de Valencia (VIU), Master en [Big Data y Data Science](https://www.universidadviu.es/master-universitario-big-data-data-science/).

La presentación está disponible en [notist](https://noti.st/immavalls).

## Pre-requisitos

- Docker y Docker Compose. Se ha probado con docker versión 19.03.8 y docker-compose 1.26.0-rc3.
  - Usuarios de Windows y Mac users tendrán Compose instalado automáticamente con Docker para [Windows](https://docs.docker.com/docker-for-windows/install/)/[Mac](https://docs.docker.com/docker-for-mac/install/).
  - Los usuarios de Linux puede leer las [instrucciones de instalación](https://docs.docker.com/compose/install/#install-compose) o pueden instalar vía `pip`:
  
    ```shell
    pip install docker-compose
    ```

- Un mínimo de 4GiB de RAM para contenedores. Los usuarios de Mac y Windows deben configurar su máquina virtual Docker para disponer de ese mínimo.

    ![Docker VM memory settings](./doc/img/docker-vm-memory-settings.png)

- Debido a que que por defecto la [memoria virtual](https://www.elastic.co/guide/en/elasticsearch/reference/7.3/vm-max-map-count.html) no es suficiente, los usuarios de Linux deben ejecutar el siguiente comando como `root`:

```
sysctl -w vm.max_map_count=262144
```

## Elastic Stack

- Instrucciones para la demo en el siguiente [documento](./doc/pdf/Introduccion-Stack-Elastic-Demos.pdf).

## Machine Learning

- Instrucciones para la demo en el siguiente [documento](./doc/pdf/Machine-Learning-Elasticsearch-demos.pdf). 

## Finalizar

Al terminar, eliminar el entorno creado con el siguiente comando.

```shell
docker-compose down -v
```
