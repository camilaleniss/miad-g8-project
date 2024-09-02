# MIAD G8 - Proyecto de Clasificación de Clases Sociales en Colombia

Este repositorio contiene el código, datos y recursos relacionados con nuestro proyecto que explora la clasificación de clases sociales en Colombia utilizando algoritmos de aprendizaje no supervisado. Basado en datos del **DANE** y aplicado con técnicas como **K-means**, **clustering jerárquico** y **DBSCAN**, este proyecto busca identificar patrones y agrupamientos naturales dentro de la población colombiana.

## Estructura del Repositorio

- **`data/`**  
  Contiene el dataset inicial utilizado en el análisis exploratorio. Este dataset fue extraído de los datos abiertos del DANE y contiene variables socioeconómicas clave como ingresos, ocupación, nivel educativo y edad.

- **`research/`**  
  Incluye los papers relevantes utilizados para fundamentar el trabajo, proporcionando el marco teórico y metodológico de apoyo al proyecto.

- **`Entrega_1_Proyecto.pdf`**  
  Aquí encontrarás el documento inicial del proyecto, que presenta la motivación, metodología y objetivos del trabajo, además del análisis descriptivo de los datos.

- **`Entrega_1_Exploracion_datos.ipynb`**  
  El notebook donde se realizó el análisis exploratorio de los datos. Este notebook incluye gráficos y estadísticas que ayudan a comprender las características del dataset y las relaciones entre las variables.

## Objetivos

El objetivo principal es explorar y comparar agrupamientos naturales de la población colombiana utilizando algoritmos de aprendizaje no supervisado y contrastarlos con la clasificación oficial del **DANE**. Este análisis tiene implicaciones para mejorar las políticas públicas y adaptar las intervenciones sociales a las verdaderas necesidades de la población.

## Requisitos

Asegúrate de tener instalados los siguientes paquetes antes de ejecutar los notebooks:

- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`
- `seaborn`

Puedes instalarlos utilizando pip:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
