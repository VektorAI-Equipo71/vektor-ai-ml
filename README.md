# ✈️ Vektor AI - Machine Learning Model

Modelo predictivo para estimar retrasos de vuelos usando Random Forest.

## Set de Datos

Para formar el set de datos propio se recurrió a datos de aerolíneas del Bureau of Transportation Statistics (Consultado el 17 de dicimebre de 2025) del Departamento de transporte de Estados Unidos (United States Department of Transportation). 

- Se decidió tomar un año de datos, desde octubre de 2024 a septiembre de 2025 e inicialmente trabajar con las 109 variables de la base de datos:
https://www.kaggle.com/datasets/spmv1980/hackaton-2025-equipo-71?select=flight_delays_one_year.csv

- Por motivos de procesamiento, se trabajó de forma preliminar con sólo dos aerolíneas para que el set de datos pudiese ser leído en la cuenta gratuita de Google Colab:
https://www.kaggle.com/datasets/spmv1980/hackaton-2025-equipo-71?select=flight_delays_one_year_2a.csv

- Una vez que se realizaron algunos modelos preliminares, se procedió a trabajar con las 15 aerolíneas disponibles en ese rango de tiempo, pero con variables seleccionadas:
https://www.kaggle.com/datasets/spmv1980/hackaton-2025-equipo-71?select=df_procesado_todas+las+aerolneas.csv

## 🚀 Stack Tecnológico
- Python 3.9+
- pandas, numpy, scikit-learn
- Jupyter Notebook

## 📁 Estructura
```
├── notebooks/          # Jupyter notebooks (EDA, training)
├── data/              # Datasets
├── models/            # Modelos serializados
├── src/               # Scripts Python
└── requirements.txt   # Dependencias
```

## 🔧 Instalación
```bash
pip install -r requirements.txt
```

## 👥 Team
- Líder Técnico DS: Sofía Marínez Véjar
- Data Scientists: Karen Brenes; Mario Baillon; Carolina Guerrero; Ronald Varela; Cristian Maje; Kevin Lemos.
