# Parcial 1 Gestión de Datos:

Nikolas Rodriguez Alfonso

Realizando un análisis exploratorio del dataset se dan respuesta a las siguientes preguntas:

1.¿Qué tipo de variables tiene el dataset? Detalle el tipo de variable de cada columna.

![Test Image 4](https://github.com//NikolasRodriguezA/Gestion_Datos/tree/main/img/Variables.PNG)

#   Column                       Non-Null Count  Dtype  
---  ------                       --------------  -----  
 0   gender                       953 non-null    object 
 1   race/ethnicity               955 non-null    object 
 2   parental level of education  940 non-null    object 
 3   lunch                        946 non-null    object 
 4   test preparation course      959 non-null    object 
 5   math score                   949 non-null    float64
 6   reading score                952 non-null    float64
 7   writing score                951 non-null    float64
dtypes: float64(3), object(5)
memory usage: 62.6+ KB


2. ¿Qué tipo de problemas de calidad de datos logra identificar? Defina e implemente las estrategias de limpieza de datos que correspondan.


La variable con más datos nulos es el nivel de educación parental con aproximadamente un 6%

Debido a los análisis requeridos más adelante se realiza una limpieza de datos faltantes para las variables númericas, realizando un fillna()

Verificación de valores atípicos o mal diligenciados en las variables categoricas

Se puede observar que las variables contienen sus categorías bien definidas y sin valores mal diligenciados o sin sentido

![Test Image 2](https://github.com//NikolasRodriguezA/Gestion_Datos/tree/main/img/Educación.PNG)
![Test Image 3](https://github.com//NikolasRodriguezA/Gestion_Datos/tree/main/img/Genero.PNG)
![Test Image 4](https://github.com//NikolasRodriguezA/Gestion_Datos/tree/main/img/Raza.PNG)
![Test Image 4](https://github.com//NikolasRodriguezA/Gestion_Datos/tree/main/img/Relaciones.PNG)


3. ¿En qué asignatura en promedio los estudiantes obtuvieron un mejor puntaje? ¿Hay evidencia de algún sesgo en la distribución de dichos puntajes?

Promedio en Matemáticas: 66.26567164179104
Promedio en Lectura: 69.54477611940298
Promedio en Escritura: 68.47164179104477

el mayor promedio es: 69.54477611940298Y corresponde a Lectura

![Test Image 4](https://github.com//NikolasRodriguezA/Gestion_Datos/tree/main/img/Promedios.PNG)

![Test Image 4](https://github.com//NikolasRodriguezA/Gestion_Datos/tree/main/img/Dist1.PNG)

4. ¿Existe alguna correlación entre los puntajes obtenidos en las tres asignaturas?

![Test Image 4](https://github.com//NikolasRodriguezA/Gestion_Datos/tree/main/img/Relaciones.png)

Realizando un análisis de dispersión se logra observar una fuerte relación lineal entre las tres variables de calificación, razón por la cual se decide hacer un análisis de correlación de spearman encontrando que entre las tres tienen correlación por encima del 80%

![Test Image 4](https://github.com//NikolasRodriguezA/Gestion_Datos/tree/main/img/corr.png)

5. ¿Hay alguna diferencia observable en los puntajes de la asignatura de matemáticas entre géneros? ¿Qué género obtuvo en promedio los mejores puntajes?

Según un anpalisis de promedios, distribución y diagrama de caja se puede observar que el genero "male" tiene una puntuación mayor que las otras dos categorías: 

![Test Image 4](https://github.com//NikolasRodriguezA/Gestion_Datos/tree/main/img/box1.png)

![Test Image 4](https://github.com//NikolasRodriguezA/Gestion_Datos/tree/main/img/box2.png)

6. ¿Qué nivel de escolaridad tienen los padres de los estudiantes que obtuvieron un puntaje por encima del percentil 85 en la asignatura de escritura? ¿Cómo se distribuye la escolaridad entre esta población?.

![Test Image 4](https://github.com//NikolasRodriguezA/Gestion_Datos/tree/main/img/Punto6.PNG)


7. ¿Qué porcentaje de los estudiantes obtuvieron puntajes iguales o superiores a 90 en las tres asignaturas? De estos estudiantes¿que porcentaje estudió para los exámenes?

 Del 100% de estudiantes solo el: 1.9% Aprobo las 3 materias por encima de 90

![Test Image 4](https://github.com//NikolasRodriguezA/Gestion_Datos/tree/main/img/Punto7.PNG)
