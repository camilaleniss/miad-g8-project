# MIAD G8 - Proyecto de Clasificación de Clases Sociales en Colombia

Este repositorio contiene el código, datos y recursos relacionados con nuestro proyecto que explora la clasificación de clases sociales en Colombia utilizando algoritmos de aprendizaje no supervisado. Basado en datos del **DANE** y aplicado con técnicas como **K-means**, **clustering jerárquico** y **DBSCAN**, este proyecto busca identificar patrones y agrupamientos naturales dentro de la población colombiana.

## Estructura del Repositorio

- **`data/`**  
  Contiene los datasets utilizados en el proyecto. Inicialmente contiene el dataset para la limpieza, fue extraído de los datos abiertos del DANE y contiene variables socioeconómicas clave como ingresos, ocupación, nivel educativo y edad. Luego de la limpieza, se exportó otro dataset para correr los modelos sobre este.

- **`research/`**  
  Incluye los papers relevantes utilizados para fundamentar el trabajo, proporcionando el marco teórico y metodológico de apoyo al proyecto.

- **`docs/`**  
  Aquí encontrarás los documentos de entrega inicial y final del proyecto. En el doc inicial podrás encontrar  documento inicial la motivación, metodología y objetivos del trabajo, además del análisis descriptivo de los datos. Mientras que en el documento final se encuentran los resultados y conclusiones del proyexto

- **`notebooks/`**  
  Contiene los notebooks para el paso a paso del proyecto:
  - **Notebook de análisis exploratorio:** Este notebook incluye gráficos y estadísticas que ayudan a comprender las características del dataset y las relaciones entre las variables.
  - **Notebook de limpieza de datos:** En este notebook encuentra todo el proceso de imputación, validación y mapeo que comprende la limpieza de los datos, y las decisiones tomadas en esta fase.
  - **Notebooks de modelos:** En este notebook se encuentra todos los modelos aplicados para resolver el problema, PCA, y conclusiones sobre el proyecto.

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



## DVC

Nuestra herramienta de control de versiones de datos es DVC. Para poder trabajar con los datos originales, los cuales se encuentran almacenados en S3 se debe instalar DVC ejecutando:

- `pip install dvc`
- `pip install "dvc[s3]`

Para descargar los datos localmente requeriras tener configurado:
Opcion 1: Instalar aws cli
* curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o ~/"awscliv2.zip"
* sudo apt install unzip
* unzip ~/awscliv2.zip -d ~/
* sudo ~/aws/install
* Configurar credenciales de AWS
* aws configure --> Se debe insertar la secret key y la acess key. La region debe ser us-east-1
* aws configure set aws_session_token SESSIONTOKEN
Opcion 2: definir variables de entorno (Si no se instalo AWS CLI)
export AWS_SECRET_ACCESS_KEY=
export  AWS_ACCESS_KEY_ID=
export  AWS_SESSION_TOKEN=

## MLflow

Asegúrate de tener instalados los siguientes paquetes para poder registrar los experimentos de los modelos en MLflow:

* pip3 install mlflow
Ejecute la interfaz grafica de MLFLOW: mlflow ui —> Queda en el la dirección: http://localhost:5000/