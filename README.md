# 🏦 Predicción de Abandono de Clientes (Bank Customer Churn)

## 📌 Descripción del Proyecto
Este proyecto consiste en el desarrollo de un **pipeline de Machine Learning** de extremo a extremo para predecir la probabilidad de que un cliente abandone el banco (*churn*). El objetivo de negocio es permitir a la entidad financiera identificar clientes en riesgo y diseñar estrategias de retención proactivas.

El proyecto no solo entrena un modelo, sino que sigue las **buenas prácticas de ingeniería de software**: modularización del código, tests unitarios, gestión de dependencias y documentación automatizada.

## 🛠️ Stack Tecnológico
*   **Lenguaje:** Python 3.x
*   **Análisis y Procesamiento:** Pandas, Scikit-learn
*   **Deep Learning:** PyTorch, PyTorch Lightning
*   **Optimización de Hiperparámetros:** Optuna
*   **Testing:** Pytest
*   **Documentación y Reportes:** Quarto
*   **Despliegue:** Cloudflare Workers (Serverless) mediante `wrangler.toml`

## 📂 Estructura del Proyecto
```text
├── data/               # Datos crudos (raw) y procesados (processed)
├── src/                # Código fuente del modelo
│   ├── preprocessing.py # Limpieza y transformación de datos
│   ├── model.py         # Arquitectura de la red neuronal
│   ├── train_lightning.py # Entrenamiento con PyTorch Lightning
│   └── optuna_search.py # Búsqueda de hiperparámetros
├── tests/              # Pruebas unitarias del pipeline (Pytest)
├── _quarto.yml         # Configuración de la documentación (Quarto)
├── requirements.txt    # Dependencias del proyecto
└── wrangler.toml       # Configuración para despliegue Serverless
