# Catalonia-Traffic-Accidents-ML
Machine learning models (SVM, k-NN, Decision Trees) to predict traffic accident severity in Catalonia using open data (2010–2020).

# Predicting Traffic Accident Severity in Catalonia (2010–2020)

[English](#english) | [Català](#català) | [Español](#español)

---

<a name="english"></a>
## English

This project evaluates and compares supervised machine learning models to predict traffic accident fatalities in Catalonia using open data provided by the Servei Català de Trànsit.

### Project Overview
* **Objective:** Predict a binary target variable (`Morts_Binaria`) indicating accident severity based on 9 selected features, including road type, speed limits, regional location, and temporal factors.
* **Data Source:** Historical traffic accident records in Catalonia (2010–2020).

### Methodology & Models
Several supervised learning algorithms were implemented, hyperparameter-tuned, and evaluated:
* **Support Vector Machines (SVM):** Tested with linear, polynomial, and radial basis function (RBF) kernels.
* **k-Nearest Neighbors (k-NN):** Evaluated across various distance metrics and neighbor counts.
* **Decision Trees:** Optimized using both Gini impurity and Information Gain (Entropy) criteria.

### Key Results
* **Best Performing Model:** The **Decision Tree** (using the Gini criterion and a maximum depth of 4) achieved the best overall performance, yielding a ROC-AUC of **0.6329** and a Matthews Correlation Coefficient (MCC) of **0.1896**, effectively handling class imbalance better than models like k-NN.
* **Predictive Insights:** Feature importance analysis revealed that the distinction between urban and interurban roads (serving as the root node) alongside speed limits are the most critical predictors of accident fatality.

### Tech Stack
* **Language:** Python
* **Libraries:** Scikit-Learn, Pandas, NumPy, Matplotlib, Seaborn

---

<a name="català"></a>
## Català

Aquest projecte avalua i compara models d'aprenentatge automàtic supervisat per predir la fatalitat d'accidents de trànsit a Catalunya utilitzant dades obertes del Servei Català de Trànsit.

### Visió General del Projecte
* **Objectiu:** Predir una variable objectiu binària (`Morts_Binaria`) que indica la gravetat de l'accident a partir de 9 variables seleccionades, incloent-hi el tipus de via, els límits de velocitat, la comarca i factors temporals.
* **Font de Dades:** Registres històrics d'accidents de trànsit a Catalunya (2010–2020).
### Metodologia i Models
Es van implementar, optimitzar i avaluar diversos algorismes d'aprenentatge supervisat:
* **Màquines de Vector de Suport (SVM):** Provades amb nuclis lineal, polinòmic i radial (RBF).
* **k-Nearest Neighbors (k-NN):** Avaluats amb diverses mètriques de distància i nombre de veïns.
* **Arbres de Decisió:** Optimitzats amb criteris d'impuresa de Gini i Entropia.

### Resultats Clau
* **Millor Model:** L'**Arbre de Decisió** (criteri Gini i profunditat màxima de 4) va aconseguir el millor rendiment general, amb un ROC-AUC de **0,6329** i un coeficient de correlació de Matthews (MCC) de **0,1896**, gestionant millor el desequilibri de classes que models com k-NN.
* **Conclusions Predictives:** L'anàlisi d'importància de variables va demostrar que la distinció entre vies urbanes i interurbanes (actuant com a node arrel) i els límits de velocitat són els predictors més crítics.

### Tecnologies
* **Llenguatge:** Python
* **Llibreries:** Scikit-Learn, Pandas, NumPy, Matplotlib, Seaborn

---

<a name="español"></a>
## Español

Este proyecto evalúa y compara modelos de aprendizaje automático supervisado para predecir la fatalidad de accidentes de tráfico en Cataluña utilizando datos abiertos del Servei Català de Trànsit.

### Resumen del Proyecto
* **Objetivo:** Predecir una variable objetivo binaria (`Morts_Binaria`) que indica la gravedad del accidente basándose en 9 variables seleccionadas, incluyendo tipo de vía, límites de velocidad, comarca y factores temporales.
* **Fuente de Datos:** Registros históricos de accidentes de tráfico en Cataluña (2010–2020).

### Metodología y Modelos
Se implementaron, optimizaron y evaluaron diversos algoritmos de aprendizaje supervisado:
* **Máquinas de Vectores de Soporte (SVM):** Probadas con núcleos lineal, polinómico y radial (RBF).
* **k-Nearest Neighbors (k-NN):** Evaluados con diferentes métricas de distancia y número de vecinos.
* **Árboles de Decisión:** Optimizados usando criterios de impureza de Gini y Entropía.

### Resultados Clave
* **Mejor Modelo:** El **Árbol de Decisión** (con criterio Gini y profundidad máxima de 4) logró el mejor rendimiento general, obteniendo un ROC-AUC de **0,6329** y un Coeficiente de Correlación de Matthews (MCC) de **0,1896**, manejando mejor el desbalance de clases que k-NN.
* **Perspectivas Predictivas:** El análisis de importancia de características reveló que la distinción entre vías urbanas e interurbanas (actuando como nodo raíz) junto con los límites de velocidad son los predictores más críticos.

### Stack Tecnológico
* **Lenguaje:** Python
* **Librerías:** Scikit-Learn, Pandas, NumPy, Matplotlib, Seaborn
