# especializacionbigdata
## Pipeline & JObs
### Pipeline Azure Data Factory
El pipeline presentado corresponde a un flujo de procesamiento de datos bajo una arquitectura tipo Medallion en Databricks, compuesto por cuatro notebooks encadenados secuencialmente. El proceso inicia con NB-INGEST-DATA, encargado de la ingesta y carga de datos desde las fuentes origen hacia la capa inicial del ecosistema. Posteriormente, NB-SILVER-DATA realiza procesos de depuración, validación, normalización y transformación de los datos para garantizar calidad y consistencia. Luego, NB-GOLD-DATA consolida y estructura la información de negocio mediante agregaciones y modelos analíticos optimizados para consumo corporativo. Finalmente, NB-GOLD-MODEL ejecuta la generación de modelos, métricas o artefactos analíticos avanzados sobre la información refinada de la capa Gold.

![image_1779492313259.png](./image_1779492313259.png "image_1779492313259.png")

### Job Dbw
El job presentado implementa un flujo de procesamiento de datos especializado bajo una arquitectura medallion en Databricks, orquestado mediante tareas secuenciales con dependencias controladas. La etapa Bronce ejecuta el notebook NB-BRONZE-INGEST-DATA, responsable de la ingesta inicial y almacenamiento de datos crudos provenientes de las fuentes transaccionales. Posteriormente, la capa Silver ejecuta NB-SILVER-PROCESS-DATA sobre un entorno Serverless, donde se aplican procesos de limpieza, homologación, validaciones de calidad y transformaciones de negocio para estructurar la información.

La siguiente etapa, Gold, ejecuta NB-GOLD-LOAD-DATA, encargado de consolidar y disponibilizar datasets curados y optimizados para consumo analítico y modelos avanzados. Finalmente, el proceso MODEL_PREDICT_RATING ejecuta el notebook NB-MODEL-PREDICT, donde se realiza la inferencia o ejecución del modelo predictivo sobre la información refinada de la capa Gold, permitiendo generar resultados analíticos y predicciones requeridas.

## Pruebas
### Pruebas Pipeline Azure Data Factory

![image_1779492396808.png](./image_1779492396808.png "image_1779492396808.png")

### Pruebas Job Dbw
![image_1779492401252.png](./image_1779492401252.png "image_1779492401252.png")

## Power BI:
Link: https://unaulaedu.sharepoint.com/:u:/s/BigData/IQCdNtpqS1GbRJR1cCFuU2LzAcGw32uAsx4M65CRiJCcs7w?e=F7dEwv