![GRUPO 5](https://github.com/melibraile/Entrega-Final-Grupo-5/assets/140036213/862f0410-efd5-424b-8208-00de09ab1a72)
## Integrantes 👩‍💻
* **Mariela Abrego**
* **Melisa Braile** 
* **Tania Damiani**
* **Mariana Grau**
* **Micaela Melian**

## Contenido ✒️
1. [Descripción del proyecto](#id1)
2. [Datasets](#id2)
3. [Herramientas](#id3)
4. [Conclusiones](#id4)


<div id='id1' />
  
## Descripción del proyecto  📌

<p align="justify">
Trabajamos en 2 proyectos:
  
* **Netflix**
En este proyecto trabajamos con datos de la plataforma Netflix. 
Netflix es un servicio de streaming que ofrece una amplia gama de películas, series y documentales de alta calidad, disponibles en prácticamente cualquier dispositivo conectado a internet.  
El objetivo del proyecto es predecir cuántas semanas va a estar un título top ten en Netflix en las diferentes regiones, teniendo en cuenta el género, el content type y el tipo de estación a la que pertenecen. 
Para el análisis utilizamos un modelo de aprendizaje supervisado.
  
* **Fifa** 
En este proyecto trabajamos sobre datos de Career Mode del videojuego FIFA 15 a FIFA 22. 
El objetivo del proyecto es agrupar a los jugadores en clusters basados en sus características, como la posición, la puntuación general, la edad, el valor de mercado, etc. Este dato se encuentre en la feature overall.El objetivo es analizar esta variable con el valor de venta en euros de los jugadores y comparar resultados. Se analizará cómo estas variables se relacionan con el valor de venta en euros de los jugadores, con el fin de identificar patrones y tendencias que puedan influir en la valoración y comercialización de los jugadores. Para el análisis utilizamos un modelo de aprendizaje no supervisado
</p>

<div id='id2' />
  
## Datasets 📄

<p align="justify">
  
* **Netflix** El dataset proviene directamente de Netflix. Consta de 2 archivos, uno de ellos con los datos y caracterisiricas de los títulos y series y el otro con información adicional.
 *  netflix_modelo.xlsx: dataset utilizado para los modelos

| Features  | Descripcion |
| ------------- | ------------- |
| region  | indica continente en el cual se proyecta la serie o película  |
| country_name | nombre del país en el cual se proyecta la serie o película  |
| country_iso2  | código ISO del país (Código de dos letras para identificar países según la norma ISO 3166-1)  |
| week | semana en la cuál la película o serie se encontró en el TOP10 |
| category  | indica la clasificación de los títulos en Serie o Película <li>**Movie**</li><li>**Series**</li>   | 
| weekly_rank  |indica la cantidad de semanas que el título estuvo en el TOP10  |
| show_title  | nombre de la serie o película |
| season_title | para el caso de las series indica el título de cada temporada  |
| cumulative_weeks_in_top_10  | cantidad de semanas acumuladas que el título estuvo en el TOP10  |
| Realease Year  | año de lanzamiento de la serie o película |
| Genre | género que identifica la serie o película |   


entorno.xlsx: varios datases con información adicional al dataset principal. Estos dataset aportaron valor al análisis inicial de los datos.



* **Fifa**  El dataset contiene infomración detallada de los jugadores para el Career Mode del videojuego FIFA 15 a FIFA 22. Estos datos permiten realizar múltiples comparaciones para los mismos jugadores a lo largo de las últimas 8 versiones del videojuego.
Los datos se han extraído del sitio web disponible públicamente en sofifa.com.
Se describen a continuación las principales features usadas para el análisis

| Features  | Descripcion |
| ------------- | ------------- |
| sofifa_id  | id |
| player_url| url con la información  |
| short_name  | nombre corto del jugador  |
| long_name | nombre detallado del jugado|
| player_positions  | posición en la que juega <li>**RW - Right Winger (Extremo Derecho)**</li><li>**ST - Striker (Delantero Centro)**</li><li>**CF - Center Forward (Delantero Centro)**</li><li>**CAM - Central Attacking Midfielder (Centrocampista Ofensivo)**</li><li>**CDM - Central Defensive Midfielder (Centrocampista Defensivo)**</li><li>**CM - Central Midfielder (Centrocampista Central)**</li><li>**LM - Left Midfielder (Centrocampista Izquierdo)**</li><li>**RM - Right Midfielder (Centrocampista Derecho)**</li><li>**LW - Left Winger (Extremo Izquierdo)**</li><li>**GK - Goalkeeper (Portero)**</li> | 
| overall  |valoración general o puntaje que se asigna para representar la calidad general del jugador en el videojuego FIFA. Es una medida compuesta que tiene en cuenta múltiples habilidades y atributos del jugador, como velocidad, habilidad con el balón, capacidad de disparo, defensa, entre otros  |
| value_eur | valor de venta del jugador en euros |
| wage_eur  | salario o sueldo que gana el jugador |
| age  | edad del jugador |
| dob | fecha de nacimiento | 
| height_cm  | altura |
| club_team_id| is del club en el que juga  |
| club_name  | nombre del club en el que juega  |
| league_name | liga en la que juega|
| league_level  | nivel de liga   | 

</p>

<div id='id3' />
  
## Herramientas 🛠️

<p align="justify">
  
![Jupyter_logo](https://github.com/melibraile/Entrega-Final-Grupo-5/assets/140036213/362b39c6-b196-45e4-9d06-e104dd323b8e)   ![python-Centro-REDES](https://github.com/melibraile/Entrega-Final-Grupo-5/assets/140036213/5ed31d48-cea5-4b10-b4ae-e896d22cb05c)



![Pandas_logo](https://github.com/melibraile/Entrega-Final-Grupo-5/assets/140036213/ebccefc1-38a5-4109-8507-df8e449c368d)   ![illu_numpy_blog-125](https://github.com/melibraile/Entrega-Final-Grupo-5/assets/140036213/5a333727-2f71-4297-9b42-92a40f60ce16)


![matplotlib](https://github.com/melibraile/Entrega-Final-Grupo-5/assets/140036213/be7cb2f9-94d4-4039-96f7-37271dae69c9)    ![seaborn](https://github.com/melibraile/Entrega-Final-Grupo-5/assets/140036213/e51bd558-90fd-4314-b7bd-78fb38e7eca3)

<div id='id4' />
  
## Conclusiones 📉

**Netflix** 
Utilizamos el modelo de Regresión Lineal, ya que nuestro objetivo es predecir cuántas semanas va a estar un título top ten en las diferentes regiones, a partir de los datos históricos que nos brinda la plataforma. Las variables independientes que utilizaremos son "region, "content type","cumulative_weeks_in_top_10" y "genre". La primera es la variable cuantitativa (x) mientras que el resto son el target (y). 
El Mean Absolute Error (MAE)nos dió 0.80.


En este proyecto de Netflix, el uso del árbol de decisiones revela las variables más influyentes con menor margen de error. Esta visualización nos permite seleccionar aquellas que explican mejor el modelo, proporcionando información precisa para decisiones basadas en datos más cercanos a la realidad. En la parte superior del árbol, se detallan las variables que maximizan la capacidad del modelo para realizar predicciones precisas.

Tambien incluimos el modelo de regresión Random Forest, se observa un rendimiento insatisfactorio con un Mean Squared Error (MSE) de 45.58 y un R-squared (R2) de 0.20 en el conjunto de prueba. Estos datos nos muestra que el modelo no explica o no se ajusta lo sufieciente para poder tomar decisiones.

**Fifa** 
Utilizamos modelo KMEANS. Este modelo nos permitió agrupar a los jugadores según el overall, es decir, el desempeño que tienen los mismos y su valor económico establecido en el mercado. Los que tienen un rendimiento mayor tienen un valor de transferencia mayor.

</p>
