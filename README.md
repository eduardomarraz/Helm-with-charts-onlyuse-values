## Estructura del Proyecto

```plaintext
.
|-- Chart.yaml
|-- README.md
|-- templates
|   |-- NOTES.txt
|   |-- _helpers.tpl
|   |-- deployment.yaml
|   |-- service.yaml
|   `-- serviceaccount.yaml
`-- values.yaml

1 directory, 8 files

```


Cambiar el archivo values.yaml para cambiar el servicio que se desea levantar, en el caso de apache con "httpd" y el tag adecuado
y en el caso de nginx poner "nginx"

```bash

helm install demo . -f values.yaml

helm upgrade demo . -f values.yaml

```