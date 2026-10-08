<img src="https://mmss.iimas.unam.mx/dmmss/wp-content/uploads/2026/02/cropped-LogoUNAM_IIMAS_Negro50-scaled-2.png" width="200"/>

### Datos Masivos II
# Práctica: Reglas de asociación y patrones frecuentes
> Equipo Tres: Castrillo Cruz Karen Arlet, Ramos González Nadia, Zamora Antiga Ángel Javier.

---

El presente repositorio identifica reglas de asociación y patrones frecuentes en tres conjuntos de datos, usando en cada uno el algoritmo más adecuado a la estructura de sus datos:

| Carpeta | Dataset | Algoritmo |
|---|---|---|
| `Online Retail II/` | [Online Retail II (UCI)](https://archive.ics.uci.edu/dataset/502/online+retail+ii), años 2009-2010 y 2010-2011 | _por definir_ |
| `Titanic/` | [Titanic (Kaggle)](https://www.kaggle.com/competitions/titanic/data), `train.csv` | FP-Growth |
| `FIFA/` | [FIFA (SPMF)](https://www.philippe-fournier-viger.com/spmf/index.php?link=datasets.php) | PrefixSpan |

```text
T2_DMII/
├── Online Retail II/
├── Titanic/
│   ├── notebooks/
│   │   ├── 01_eda_calidad_preprocesamiento.ipynb   # perfilado, calidad y transformación
│   │   └── 02_fpgrowth_reglas_asociacion.ipynb     # FP-Growth y reglas
│   └── data/                                       # no incluida: ver Titanic/README.md
└── FIFA/
    ├── prefixspan_reglas_asociacion.ipynb          # Aplicación del algoritmo y análisis general de distribución de transacciones
    └── data/                                       # no incluida: ver FIFA/README.md
```

Los datos no se incluyen en el repositorio; cada carpeta explica cómo obtenerlos.

> Instituto de Investigaciones en Matemáticas Aplicadas y en Sistemas, Universidad Nacional Autónoma de México. Octubre, 2026