# Titanic: reglas de asociación con FP-Growth

1. Descarga `train.csv`, `test.csv` y `gender_submission.csv` de
   https://www.kaggle.com/competitions/titanic/data y colócalos en `Titanic/data/`.
2. Instala las dependencias: `pip install -r requirements.txt` (desde la raíz del repositorio).
3. Ejecuta en orden:
   - `notebooks/01_eda_calidad_preprocesamiento.ipynb` (genera `data/processed/`).
   - `notebooks/02_fpgrowth_reglas_asociacion.ipynb`.

Solo `train.csv` entra al análisis; la justificación está en la sección 1 del notebook 1.