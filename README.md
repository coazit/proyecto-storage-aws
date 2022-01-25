Diseñar una arquitectura de almacenamiento para la empresa de seguros. Además, debes implementar una prueba de concepto que como mínimo cuente con lo siguiente:

    2 buckets en diferentes regiones.

    Replicación de archivos entre las regiones.

    Pruebas de replicación entre regiones.

    Configuración del bucket principal con las siguientes funcionalidades:
    Versionamento.
    Encriptación con KMS.
    Ciclo de vida de la siguiente forma (no para objetos versiones anteriores):
        Objetos mayores a 2 meses pasan a S3-IA.
        Objetos con 6 meses de antigüedad pasan a Glacier.
        Objetos con 2 años de antigüedad deben borrarse.

    Crear un servidor con un volumen EBS agregado a la instancia.

    A través de la CLI consultar los buckets generados y migrar la información que se
    tiene en el EBS al bucket usando la CLI.

    Genera un snapshot del volumen y mígralo a la región en donde se encuentra el bucket secundario.

