# Análisis Comparativo de Sentimientos: Modelos Tradicionales vs. Transformers

Este repositorio contiene el desarrollo del **Proyecto 1** para el laboratorio de modelos avanzados de Procesamiento de Lenguaje Natural (PLN) en el contexto de **JENNER & PHIPPS**.

## 🎯 Objetivo del Proyecto
El propósito de este proyecto es diseñar, implementar y evaluar un pipeline automático de análisis de sentimientos. Se busca comparar la eficacia de los métodos estadísticos clásicos frente a los modelos de lenguaje basados en arquitectura Transformer para identificar la polaridad en comentarios de usuarios.

## 🛠️ Stack Tecnológico
* **Lenguaje:** Python 3.9+
* **Procesamiento de Texto:** `NLTK`, `SpaCy`.
* **Modelado Clásico:** `Scikit-learn` (Naive Bayes, TF-IDF).
* **Modelado Avanzado:** `Hugging Face Transformers` (BERT).
* **Análisis de Datos:** `Pandas`, `NumPy`.
* **Visualización:** `Matplotlib`, `Seaborn`.

## 📋 Metodología
El flujo de trabajo se divide en cuatro fases críticas:

1.  **Recolección y Limpieza:** Carga de datasets (Twitter/IMDb/Amazon) y preprocesamiento (eliminación de caracteres especiales, stop-words y tokenización).
2.  **Extracción de Características:** Implementación de vectorización **TF-IDF** para el modelo baseline.
3.  **Entrenamiento y Fine-tuning:**
    * **Naive Bayes:** Como modelo de referencia por su eficiencia computacional.
    * **BERT:** Como modelo de estado del arte para capturar contexto semántico profundo.
4.  **Evaluación Comparativa:** Análisis de rendimiento mediante métricas de **Precisión (Accuracy)**, **F1-Score** y **Matrices de Confusión**.

## 📂 Estructura del Repositorio
```text
├── notebooks/
│   └── sentiment_analysis_lab.ipynb    # Notebook principal con el código paso a paso
├── data/
│   └── dataset_sentimientos.csv        # Dataset utilizado para el entrenamiento/test
├── requirements.txt                    # Dependencias necesarias para el proyecto
└── README.md                           # Descripción del proyecto