# Online Retail II: reglas de asociación con FP-Growth

1. Descarga el dataset de https://archive.ics.uci.edu/dataset/502/online+retail+ii (UCI, id 502), descomprime el zip y
   coloca `online_retail_II.xlsx` en `Online Retail II/data/`.
2. Instala las dependencias: `pip install -r requirements.txt` (desde la raíz del repositorio). Se necesita Python ≥ 3.12.
3. Ejecuta en orden, desde `notebooks/`:
   - `01_eda_calidad_preprocesamiento.ipynb`: EDA, calidad y preprocesamiento. Lee `../data/online_retail_II.xlsx` y
     genera `../data/processed/` con `retail_ventas.parquet`, `retail_cancelaciones.parquet` y
     `retail_precio_cero.parquet`. Leer el Excel tarda unos minutos.
   - `02_fpgrowth_reglas_asociacion.ipynb`: canastas, FP-Growth por trimestre y reglas de asociación. Lee
     `../data/processed/retail_ventas.parquet`. Tarda unos minutos por el barrido del soporte mínimo.

Solo `retail_ventas.parquet` entra al análisis de canasta (la justificación está en la sección 6.11 del notebook 1). En el
notebook 2, el minado usa solo las facturas con `Customer ID`. Las facturas sin cliente incluyen canastas gigantes casi
idénticas que provocan una explosión combinatoria en FP-Growth (sección 2.1). Además, el 4T-2009 (que solo tiene
diciembre) queda fuera del análisis por trimestre (sección 3).
