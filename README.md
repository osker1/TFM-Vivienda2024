# TFM-Vivienda2024

## Pasos para reproducir la Pipeline

## Setup Lambda
* La función lambda se debe importar en zip con las dependencias incluidas en la carpeta Lambda. Ya está en formato zip para su uso.

## Setup Secrets
* El servicio de AWS Secrets debe tener un secreto que sea: api_key_idealista
* El valor del secreto debe ser "Basic ZHZncnZ3cG9tZWtzdm02NHB3anlpZ2VmOXhpM3g4b2c6SFhLT2VtaHJNR1Vi"
* El servicio de AWS Secrets debe tener otro secreto que sea: oauth_token_idealista

## Setup S3
* Se debe crear un bucket llamado "bucket-for-requests" seguido de estas carpetas: /data/api_database/requests_json/. El path completo sería s3://bucket-for-requests/data/api_database/requests_json/

## Setup AWS Glue
* Se debe crear una base de datos llamada "delta_lake_db"
* Importar los notebooks a AWS Glue/Jobs/Notebooks.
