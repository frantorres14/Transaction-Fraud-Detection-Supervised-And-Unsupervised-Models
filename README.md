# Detección de Fraude en Tarjetas de Crédito usando modelo supervisado y no supervisado

Este proyecto implementa modelos de aprendizaje automático para detectar transacciones fraudulentas con tarjetas de crédito. Compara dos enfoques: Autoencoders (una técnica de aprendizaje profundo no supervisado) y XGBoost (un framework de boosting por gradiente). Se realiza un breve análisis exploratorio de datos y se prueban ambos modelos, demostrando que el modelo XGBoost tiene mejor desempeño para este caso debido al desbalanceo de clases.

## Visión General del Proyecto

El proyecto explora un conjunto de datos que contiene información de transacciones con tarjetas de crédito con características como:

- Distancia desde el hogar
- Distancia desde la última transacción
- Proporción respecto al precio de compra medio
- Si se utilizó un comercio recurrente
- Si se usó chip, PIN o pedido en línea
- Si la transacción fue fraudulenta (variable objetivo)

## Características Principales

- **Análisis Exploratorio Completo**: Incluye exploración de datos, análisis de distribución y visualización de correlaciones
- **Ingeniería de Características**: Aplica transformación logarítmica y estandarización a variables continuas
- **Implementación de Modelos**:
    - **Autoencoder**: Arquitectura de red neuronal con componentes de codificador/decodificador entrenados en transacciones no fraudulentas
    - **XGBoost**: Modelo de boosting por gradiente con ajuste de hiperparámetros

## Resultados

- El modelo Autoencoder tuvo dificultades para distinguir eficazmente entre transacciones fraudulentas y no fraudulentas
- El modelo XGBoost logró un excelente rendimiento:
    - Alta precisión (~99%)
    - Recall perfecto (100%)
    - Maneja exitosamente el desequilibrio de clases mediante ponderación adecuada

## Aspectos Técnicos Destacados
- Preprocesamiento de datos e ingeniería de características
- Aprendizaje profundo con TensorFlow/Keras
- Aprendizaje por ensamble con XGBoost
- Optimización de hiperparámetros usando GridSearchCV
- Manejo efectivo del desequilibrio de clases (91.26% legítimas vs 8.74% transacciones fraudulentas)
- Evaluación de modelos utilizando métricas apropiadas para clasificación desequilibrada

## Archivos

- `credit_fraud.ipynb`: Notebook Jupyter que contiene todo el análisis e implementación del modelo
- `card_transdata.csv`: Conjunto de datos con información de transacciones con tarjetas de crédito
- `best_xgboost_model.json`: Mejor modelo XGBoost guardado después del ajuste de hiperparámetros



## 📝 Licencia

Este proyecto está licenciado bajo la Licencia MIT - ver el archivo LICENSE para más detalles.



## 👨‍💻 Autor

Francisco Torres, AI developer - [@frantorres14](https://github.com/frantorres14)




## ⭐️ ¡Si te gustó, apóyame!

¡Si te gusta el proyecto, no olvides dejar una estrella en GitHub!
También puedes seguirme en mis redes para tutoriales y videos sobre IA  
TikTok: [@frantorresia](https://www.tiktok.com/@frantorresia)  
YT: [@frantorresia](https://www.youtube.com/@frantorresia)