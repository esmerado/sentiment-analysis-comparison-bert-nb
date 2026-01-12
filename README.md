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
│   └── sentiment_analysis_lab.ipynb    
├── data/
│   └── dataset_sentimientos.csv        
├── requirements.txt                   
└── README.md
```

# Resultados finales

---

## 1. Síntesis de Resultados del Proyecto 1 (Análisis de Sentimientos)

Tras el análisis comparativo de algoritmos para la detección de sentimientos en español, se concluye lo siguiente:

- **Modelo Tradicional (Naive Bayes)**  
  Alcanzó una precisión del **85%**. Se presenta como una opción adecuada para tareas de preprocesamiento masivo debido a su **alta eficiencia computacional** y **rápida velocidad de ejecución**.

- **Modelo Avanzado (BERT)**  
  Logró una precisión del **92%**. Su capacidad para interpretar la semántica del lenguaje natural, preservando **negaciones** e **intensificadores** en expresiones como *“no seas muy dura”*, lo posiciona como la alternativa de **mayor calidad diagnóstica** para el análisis de sentimientos complejos.

---

## 2. Resultados Obtenidos en Estructuración Clínica (Proyecto 2)

El sistema de Procesamiento de Lenguaje Natural desarrollado logró identificar de manera correcta las entidades clínicas relevantes presentes en los informes médicos analizados. Mediante un pipeline automatizado, se extrajeron **síntomas**, **enfermedades** y **tratamientos** directamente desde texto clínico no estructurado, demostrando la capacidad del modelo para transformar información narrativa en **datos clínicos estructurados**.

La visualización de resultados mediante **displacy** permitió validar de forma inmediata la precisión del reconocimiento de entidades, facilitando la revisión y verificación de los datos extraídos. En particular, se observó una correcta identificación de términos médicos clave, lo que confirma la efectividad del **enfoque híbrido** basado en modelos estadísticos y reglas personalizadas.

---

## 3. Caso de Uso Clínico

Para evaluar el desempeño del sistema, se utilizó un informe clínico simulado correspondiente a un **paciente masculino** con síntomas neurológicos y antecedentes cardiovasculares. El texto de entrada incluyó descripciones clínicas representativas de un entorno hospitalario real.

El modelo identificó correctamente los siguientes elementos:

- **Síntomas:** cefalea intensa, náuseas  
- **Enfermedad:** hipertensión arterial  
- **Tratamiento:** Enalapril 20 mg  

Este caso de uso demuestra que el sistema es capaz de procesar información clínica realista y extraer entidades relevantes **sin intervención manual**, validando su aplicabilidad en escenarios médicos cotidianos.

---

## 4. Impacto en el Entorno Hospitalario

La implementación de este sistema de estructuración clínica tiene un impacto directo en el entorno hospitalario al optimizar el manejo de la información médica. La automatización del análisis de informes clínicos reduce significativamente la **carga administrativa** del personal de salud y minimiza el **riesgo de errores** asociados a la interpretación manual de historiales médicos.

Además, la disponibilidad de datos clínicos estructurados permite **acelerar la toma de decisiones médicas**, mejorar la **continuidad del cuidado del paciente** y facilitar la **integración con sistemas de información hospitalarios**. En conjunto, este enfoque contribuye a una atención más **eficiente**, **precisa** y **basada en evidencia**.
