# Pronostico-de-Generacion-de-Energia-con-Turbinas-Eolicas

🌬️ Pronóstico de Generación de Energía con Turbinas Eólicas

Este proyecto desarrolla un modelo de regresión para predecir la generación de energía eléctrica producida por turbinas eólicas, utilizando datos históricos de operación.

El objetivo es estimar la variable Power a partir de características operativas y espaciales, comparando modelos de regresión lineal y Random Forest, y analizando diferencias por ubicación de las turbinas.

🎯 Objetivos del proyecto

Analizar datos históricos de generación de energía eólica.

Explorar la relación entre variables meteorológicas/operativas y la potencia generada.

Comparar modelos de regresión:

Regresión Lineal

Random Forest Regressor

Evaluar el desempeño de los modelos mediante R².

Analizar la producción total de energía por ubicación.

🌍 Contexto

La predicción de generación eólica es clave para:

Planificación energética.

Integración de energías renovables a la red eléctrica.

Optimización operativa de parques eólicos.

Reducción de incertidumbre en mercados energéticos.

📌 Un pronóstico confiable mejora la estabilidad del sistema eléctrico y la toma de decisiones estratégicas.

📊 Dataset

Fuente: Datos históricos de entrenamiento (Train.xlsx)

Formato: Excel → Parquet

Variable objetivo: Power

Variables explicativas:

Variables operativas y de entorno

Location (identificador de parque o turbina)

Preprocesamiento aplicado

Eliminación de columnas irrelevantes (Unnamed: 0, Time).

Conversión del dataset a formato Parquet para mayor eficiencia.

Separación de variables predictoras (X) y variable objetivo (y).

🔍 Metodología
1️⃣ Exploración y limpieza de datos

Inspección de estructura y tipos de datos.

Eliminación de columnas no informativas.

Análisis de correlaciones entre variables numéricas.

2️⃣ Análisis por ubicación

Segmentación de los datos según Location.

Comparación de generación total de energía entre ubicaciones.

Visualización mediante gráficos de barras.

3️⃣ Modelado predictivo
📌 Modelos utilizados

Linear Regression

Random Forest Regressor

Ambos modelos se entrenan sobre el conjunto completo de datos para:

Comparar capacidad explicativa.

Evaluar relaciones lineales vs no lineales.

4️⃣ Evaluación

Métrica utilizada:

R² (coeficiente de determinación)

Comparación directa del desempeño entre modelos.

Random Forest muestra mayor capacidad para capturar relaciones complejas.

📈 Resultados principales

La generación de energía varía significativamente entre ubicaciones.

Existen relaciones no lineales relevantes entre las variables explicativas y la potencia generada.

Random Forest presenta un mejor ajuste global que la regresión lineal.

El análisis por ubicación permite identificar parques con mayor contribución energética.

📌 El enfoque es adecuado para escenarios reales de planificación energética y análisis de renovables.

🛠️ Tecnologías y Librerías

Python

Pandas / NumPy

Matplotlib

Scikit-learn

📁 Estructura del proyecto
├── Dataset/
│   └── Train.xlsx
├── train.parquet
├── Pronóstico de generación de energía con turbinas eólicas.py
└── README.md
▶️ Cómo ejecutar el proyecto

Clonar el repositorio:

git clone https://github.com/tu-usuario/wind-energy-forecasting.git

Instalar dependencias:

pip install pandas numpy matplotlib scikit-learn openpyxl pyarrow

Ejecutar el script:

python "Pronóstico de generación de energía con turbinas eólicas.py"
🚀 Posibles mejoras futuras

Incorporar modelos de series temporales (ARIMA, Prophet).

Feature engineering temporal (lags, medias móviles).

Validación temporal (train/test por fecha).

Ajuste de hiperparámetros del Random Forest.

Inclusión de datos meteorológicos externos.

👤 Autor

Flavia Hepp
Proyecto de Data Science aplicado a energías renovables y análisis de series temporales.
