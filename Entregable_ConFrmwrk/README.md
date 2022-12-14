***El Github incluye la descripción de la entrega (ya sea en el readme o en un documento) y contiene todos los elementos solicitados (librería utilizada, dataset usado, métrica de desempeño (valor logrado sobre el subset de prueba), predicciones de prueba (entradas, valor esperado, valor obtenido), nombre del archivo a revisar)

En esta entrega se implementa un modelo de clasificación, es este caso el de bosques aleatorios, y se hizo con ayuda de librerías. El dataset que se manejó en este código es el del clima en Australia, mostrando ciertos parámetros que podrían influir en si va a llover o no. En el código se busca predecir al tomar en cuenta las variables que se correlacionan lo más posible con el resultado. 

***Dataset 

El dataset cuenta con 23 variables, donde sus valores con categóricos completamente, esto para utilizar los modelos vistos en clase, los cuales, son de clasificación.

La variable objetivo a predecir es la de "RainTomorrow", la variable que nos da información acerca de si va a llover el siguiente día o no. Primeramente lo que se hizo en el código fue un filtrado de datos relevantes para la predicción de la variable objetivo, se hizo uso de la matriz de correlación para identificar el nivel de correlación entre las variables.


***Librerias utilizadas  

Las librerías que se utilizaron fueron:

- Matplotlib: Se usó generar gráficas y tener una mejor visualización de los datos. 
- Scikit-learn: Se usó para la construcción de nuestro modelo de clasificación, realizar nuestras predicciones y obtener las métricas. También se uso para el Cross-Validation que se implementó.
- Pandas: Se usó para la manipulación de la estructura del dataset descrito anteriormente.
- NumPy: Se usó para la manipulación de los datos, ya que, se hizo por medio de arreglos.
- Seaborn: Se usó para la la visualización de datos estadísticos, en este caso, se ocupó para la matriz de confusión.


***Métricas de desempeño (valor logrado sobre el subset de prueba)

También se presentan métricas para medir el rendimiento del modelo. La precisión del modelo fue del 85% (Se acertaron 19363 de 22585 datos) y seguido de eso se realizó un cross-validation para validar.


***Predicciones de prueba (entradas, valor esperado, valor obtenido) 
Fold:  1, Training/Test Distribución Dividida: [56179 16093], Precisión: 0.851
Fold:  2, Training/Test Distribución Dividida: [56179 16093], Precisión: 0.851
Fold:  3, Training/Test Distribución Dividida: [56179 16093], Precisión: 0.851
Fold:  4, Training/Test Distribución Dividida: [56179 16093], Precisión: 0.853
Fold:  5, Training/Test Distribución Dividida: [56180 16092], Precisión: 0.857 

Precisión del Cross-Validation: 0.853 +/- 0.002

***Nombre del archivo a revisar 

El nombre del archivo a revisar es el de "ml_framework(categóricas).py", el cual, al correrlo, ya tiene conexión al csv, llamado "weatherAUS.csv",que igual se encuentra en el repositorio.

