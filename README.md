# Resumen de Notebooks

## 1. Consulta a la API de NIST
**Objetivo:** Obtener datos de vulnerabilidades desde la API de NIST y almacenarlos en un DataFrame de Pandas.

### Pasos:
1. Realizamos una solicitud HTTP a la API de NIST.
2. Extraemos los datos en formato JSON.
3. Normalizamos la información relevante y la convertimos en un DataFrame.
4. Guardamos los datos en un archivo CSV para futuras consultas.

## 2. Tratamiento de Datos
**Objetivo:** Procesar y limpiar los datos obtenidos para facilitar su análisis y almacenamiento.

### Pasos:
1. Cargamos el archivo CSV generado en el primer notebook.
2. Convertimos las fechas a formato datetime.
3. Extraemos información clave como el año y el mes de publicación.
4. Generamos estadísticas y visualizaciones para entender la distribución de las vulnerabilidades.

## 3. Conexión a la Base de Datos y Visualización
**Objetivo:** Almacenar los datos procesados en una base de datos PostgreSQL y realizar consultas.

### Pasos:
1. Establecimos una conexión con PostgreSQL utilizando `psycopg2`.
2. Creamos una tabla para almacenar las vulnerabilidades.
3. Insertamos los datos procesados en la base de datos.
4. Realizamos una consulta para visualizar los datos almacenados y los imprimimos en pantalla desde el script.


Este flujo de trabajo nos permitió obtener, limpiar y almacenar datos de vulnerabilidades en una base de datos PostgreSQL, facilitando su posterior análisis y visualización.

