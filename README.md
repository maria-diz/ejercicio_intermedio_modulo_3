# Evaluación intermedia Modulo 3 - Maria Diz

## Los Datos:

- Varias estadísticas de la versión musical en spotify, incluido el número de streams;
- Número de visualizaciones del vídeo musical oficial de la canción en youtube.

### 1. Importa Pandas

### 2. Exploración del conjunto de datos:

- Carga el fichero, al cargarlo te aparecerá una columna llamada "Unnamed: 0". Carga el dataset sin que aparezca esta columna. Además realiza un análisis exploratorio que incluya:
    - Cuando leas el fichero, veras que no podemos ver todas las columnas, utiliza el comando correcto para poder visualizarlas todas cuando hacemos un head
    - Primeras 5 filas del dataframe
    - Últimas 5 filas del dataframe
    - 10 filas aleatorias del dataframe
    - ¿Cuántas filas y columnas tenemos en el dataframe
    - ¿Cuáles son los tipos de los datos de cada columna del dataframe
    - ¿Cuántos valores nulos tenemos por columna?
    - ¿Tenemos filas duplicadas en el dataframe ?
    - Muestra los principales estadísticos para las columnas numéricas del dataframe
    - Muestra los principales estadísticos para las columnas categóricas del dataframe

    ### 3. Preparación de los datos:
- Los nombres de las columnas empiezan con mayúsculas, pon todos los nombres de las columnas en minúsculas.
- Haciendo el análisis exploratorio te deberías haber dado cuenta de que algunas de las variables (danceability, energy, key, loudness, speechiness, acousticness, instrumentalness) no son del tipo que deberían. Esto es debido a que los decimales están establecidos como comas y no con puntos. Crea una función que nos permita cambiar esas comas por puntos para que los datos tengan el tipo correcto.
Después de haber hecho los cambios, chequea los tipos de datos. ¿Son ya del tipo correcto? En caso de que no, crea otra función o modifica la anterior para que sean de tipo float.
- Hay algunas canciones cuyo título está en mayúsulas. Crea una función para que todos los títulos estén en minúscula. Haz lo mismo para las columnas de "title" y "album".
- Algunos de los artistas tienen símbolos raros, en concreto el símbolo $. Crea una función que los reemplaze pos "s".


### 4. Filtrado de datos:
- ¿Cuáles son los valores únicos de la columna "album_type"? Crea tres dataframes diferentes, uno para cada tipo de "album_type". ¿Cuántas canciones tenemos en cada tipo?
- Usando el dataframe de los albumes que hemos creado en el ejercicio anterior. ¿Cuál es la media y la desviación estándar de "danceability", "acousticness" y "speechiness" de cada artista?. Muesrtra los resultados en tres dataframes diferentes, uno para cada métrica ("danceability", "acousticness" y "speechiness"). Ordena los resultados de mayor a menor en base a la media.
- Se quiere estudiar si existe una relación entre la cantidad de visitas que reciben los videos de música de un artista en una plataforma de streaming y la cantidad de likes que estos videos obtienen. Por lo tanto, querremos contestar a la siguiente pregunta: ¿Son aquellos artistas que tienen más visitas los que más likes tienen? Para solucionar este ejercicio deberéis:
    - Agrupa por artista y calcular la media de visitas y de likes.
    - Quedate con los 10 artistas que más visitas han tenido.
    - Quedate con los 10 artistas que más likes han tenido.
    - BONUS Haced lo mismo para los datos de tipo "single".
