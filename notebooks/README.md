# Notebooks

1) [FlightonTime_0_Armado y Elección del Set de Dataset.ipynb](https://github.com/VektorAI-Equipo71/vektor-ai-ml/blob/main/notebooks/FlightonTime_0_Armado_y_Elecci%C3%B3n_del_Set_de_Dataset.ipynb)
   
   Contiene el código para generar los distintos set de datos usados a lo largo del análisis.

2) [FlightonTime_1_EDA y Limpieza .ipynb](https://github.com/VektorAI-Equipo71/vektor-ai-ml/blob/main/notebooks/FlightonTime_1_EDA_y_Limpieza_.ipynb)
   
   Contiene el análisis exploratorio y la limpieza para el set de datos con 109 variables y dos aerolíneas, generando el set de datos. El resumen de dichos procesos se encuentra al comienzo del notebook. 

3) [FlightonTime_2_ Random_Forest - Regresión Logística.ipynb](https://github.com/VektorAI-Equipo71/vektor-ai-ml/blob/main/notebooks/FlightonTime_2__Random_Forest_Regresi%C3%B3n_Log%C3%ADstica.ipynb)
   
   Contiene el código para varias pruebas de Random Forest y Regresión Logística para dos aerolíneas. Entre las variaciones está el uso de variables candidatas, variables sólo disponibles antes del vuelo y variables recomendadas por opinión de expertos. Se aplicaron técnicas de oversampling para balancear el set de datos, "label encoding" de variables categóricas y RandomizedSearchCV para buscar los mejores hiperparámetros de los modelos. 

4) [FlightonTime_3_Random_Forest_todas_las_Aerolineas.ipynb](https://github.com/VektorAI-Equipo71/vektor-ai-ml/blob/main/notebooks/FlightonTime_3_Random_Forest_todas_las_Aerolineas.ipynb)

   Con el objetivo de mejorar la predicción, se incorporaron las quince aerolíneas presentes en el intervalo de tiempo de un año. Se realiza una análisis exploratorio y limpieza antes de aplicar un modelo de random forest para las variables seleccionadas por el experto con balanceo de datos, "label encoding" y RandomizedSearchCV.

 Para el uso de la variable de fecha ```FL_DATE```y con el objetivo de no perder información temporal cíclica se crearon las siguientes variables para evitar colinealidad y ruido:

 * mes_sin / mes_cos (Capturan estacionalidad anual (Enero ≈ Diciembre))

* dia_semana_sin / dia_semana_cos (Capturan patrón semanal (Lunes ≈ Domingo))*

* es_fin_de_semana (Señal clara y simple para Random Forest)

5) [FlightonTime _4_Random_Forest_para MVP.ipynb](https://github.com/VektorAI-Equipo71/vektor-ai-ml/blob/main/notebooks/FlightonTime__4_Random_Forest_para_MVP.ipynb)

   Este notebook contiene el modelo fue exportado para uso en Backend. Se trata de random forest con 98 estimadores, profundidad máxima de 22, cantidad mínima de hojas 16, divisiones mínimas =10, clases balanceadas. 
