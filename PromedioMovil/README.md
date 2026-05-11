Pronóstico del Número de Ocupados en las 13 Principales Ciudades de Colombia

Integrantes:
Juan Carlos Molina Lozano
Santiago Tobar Bravo
Diana Velasco Arce

📌 Descripción del Proyecto
Este proyecto tiene como objetivo realizar el pronóstico del número de ocupados en las 13 principales ciudades de Colombia mediante técnicas de series de tiempo utilizando modelos de promedio móvil (Moving Average - MA).
Se trabajó con una serie temporal mensual compuesta por 222 observaciones, comprendidas entre enero de 2001 y junio de 2019, expresadas en miles de personas ocupadas.
El análisis busca identificar la mejor ventana de promedio móvil para generar pronósticos a corto plazo y evaluar su desempeño mediante métricas estadísticas.

🎯 Objetivos
- Analizar el comportamiento histórico del número de ocupados.
- Implementar modelos de promedio móvil con diferentes ventanas.
- Evaluar el desempeño de cada modelo utilizando el RMSE (Root Mean Squared Error).
- Seleccionar el modelo con mejor capacidad predictiva.
- Generar un pronóstico para los siguientes seis meses.

📊 Dataset
La base de datos utilizada contiene información mensual del número de ocupados en las 13 principales ciudades de Colombia.

Características del dataset:
Periodo: Enero 2001 - Junio 2019
Frecuencia: Mensual
Total de observaciones: 222
Variable principal: Número de ocupados (en miles de personas)

🛠️ Tecnologías y Herramientas Utilizadas
Python
Jupyter Notebook
Pandas
NumPy
Matplotlib
Scikit-learn

📈 Metodología
1. División de los datos
La serie temporal fue dividida en:

Entrenamiento: Enero 2001 - Abril 2018 (208 observaciones)
Prueba: Mayo 2018 - Junio 2019 (14 observaciones)

2. Evaluación de modelos MA

Se evaluaron modelos de promedio móvil con ventanas entre 2 y 10 meses.

El criterio de selección fue el menor valor de RMSE obtenido sobre el conjunto de prueba.

Ventana MA	RMSE
2	          169.19
3	          181.44
4	          212.78
5	          217.05
6	          213.33
7	          204.31
8	          202.21
9	          196.83
10	        195.10

✅ Mejor Modelo Seleccionado
El modelo con mejor desempeño fue:

MA(2)
Este modelo utiliza el promedio de los dos meses más recientes para realizar el pronóstico del siguiente periodo.

🔮 Pronóstico Final
Utilizando toda la información disponible hasta junio de 2019, se obtuvieron las siguientes proyecciones:

Mes	       Pronóstico
2019-07	    10,830.50
2019-08	    10,839.25
2019-09	    10,834.88
2019-10	    10,837.06
2019-11	    10,835.97
2019-12	    10,836.52

📌 Conclusiones
El modelo MA(2) presentó el menor error de predicción entre todas las ventanas evaluadas.
El promedio móvil suaviza la serie temporal y permite generar pronósticos simples y rápidos.
El pronóstico indica una estabilidad aproximada en el número de ocupados durante el segundo semestre de 2019.
Aunque el modelo es útil para el corto plazo, tiene limitaciones:
No considera tendencia.
No incorpora estacionalidad.
No tiene en cuenta variables externas que puedan afectar el empleo.
