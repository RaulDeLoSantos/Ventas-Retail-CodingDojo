# Ventas-Retail-CodingDojo
Análisis y Predicción de Ventas en una Tienda de Retail (Core)
Desarrollo by Raul De Los Santos Caceres Penayo - 18/10/2024 

Introducción al Proyecto

En este proyecto de curso, desarrollaremos un análisis integral de un conjunto de datos de ventas de una tienda de retail. El objetivo es que los estudiantes apliquen lo aprendido en las diferentes secciones del curso, desde la manipulación básica de datos con NumPy, pasando por el análisis y visualización de datos con Pandas, hasta el uso de técnicas de machine learning para realizar predicciones. Este proyecto será una excelente adición al portafolio de los estudiantes y les permitirá demostrar su competencia en varias áreas clave de la ciencia de datos.

Dataset

Para este proyecto, utilizaremos un dataset reciente de Kaggle titulado «Retail Sales Dataset» (2023-2024). Este dataset contiene información detallada sobre las ventas diarias de diferentes productos en una tienda. Puedes descargar el dataset desde Kaggle.

Parte 1: Análisis Básico con NumPy

En esta primera parte del proyecto, los estudiantes realizarán un análisis preliminar del dataset utilizando NumPy. El objetivo es familiarizarse con los datos y realizar operaciones básicas de manipulación y análisis.

Instrucciones:

Configuración Inicial del Proyecto:
Crea un repositorio en GitHub para tu proyecto.
Configura dos ramas en tu repositorio: main y development.
Agrega un archivo README.md con una descripción del proyecto, instrucciones de instalación y uso.
Carga y Preprocesamiento de Datos:
Carga los datos del archivo CSV utilizando NumPy.
Realiza un preprocesamiento básico para asegurarte de que los datos estén limpios y listos para su análisis.
Exploración de Datos:
Calcula el total de ventas por categoría de producto.
Calcula el promedio de ventas diarias por categoría de producto.
Identifica las categorías de productos con mayores y menores ventas.
Manipulación de Datos:
Filtra los datos para mostrar solo las ventas de una categoría de producto específica.
Realiza operaciones de suma, resta, multiplicación y división en los datos para obtener estadísticas adicionales.
Guía Paso a Paso:

Configuración Inicial del Proyecto en GitHub
Crear un Repositorio en GitHub:
Ve a GitHub y crea un nuevo repositorio.
Nombra el repositorio, por ejemplo, retail-sales-analysis.
Clonar el Repositorio a tu Máquina Local:
Abre tu terminal y clona el repositorio:
git clone https://github.com/tu_usuario/retail-sales-analysis.git
cd retail-sales-analysis
Crear Ramas main y development:
Asegúrate de estar en la rama main:
git checkout main
Crea y cambia a la rama development:
git checkout -b development
Agregar un Archivo README.md:
Crea un archivo README.md con la siguiente estructura:
# Retail Sales Analysis

Este proyecto analiza y predice las ventas de una tienda de retail utilizando técnicas de ciencia de datos.

## Estructura del Proyecto

- `data/`: Contiene los archivos de datos.
- `notebooks/`: Contiene los notebooks de Jupyter para el análisis.
- `src/`: Contiene el código fuente del proyecto.
- `README.md`: Este archivo.

## Instrucciones de Instalación

1. Clona el repositorio: `git clone https://github.com/tu_usuario/retail-sales-analysis.git`
2. Instala las dependencias: `pip install -r requirements.txt`

## Uso

Ejecuta los notebooks de Jupyter en la carpeta `notebooks` para realizar el análisis de los datos.
Hacer un Commit y Push de los Cambios:
Agrega y comitea los cambios:
git add README.md
git commit -m "Add README.md"
HINT. Carga de datos con Numpy
import numpy as np

def cargar_datos(ruta_archivo):
    # Carga los datos del archivo CSV utilizando NumPy
    datos = np.genfromtxt(ruta_archivo, delimiter=',', skip_header=1)
    return datos

if __name__ == "__main__":
    ruta_archivo = '../data/retail_sales.csv'
    datos = cargar_datos(ruta_archivo)
    print(datos)
