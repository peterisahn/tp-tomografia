# Métodos Computacionales - Reconstrucción y Regularización de Imágenes Tomográficas

Repositorio con el desarrollo, implementación y análisis de métodos numéricos para la reconstrucción de imágenes tomográficas, realizado para la materia **Métodos Computacionales**.

El trabajo aborda un problema inverso: reconstruir una imagen a partir de mediciones obtenidas mediante rayos que atraviesan sus píxeles. Para ello, se utilizan herramientas de álgebra lineal, mínimos cuadrados, optimización numérica y regularización, analizando cómo influyen la cantidad de mediciones y el ruido en la calidad de las reconstrucciones.

## Contenido

- **Modelado matemático de la tomografía:**
  - Representación de imágenes como vectores de atenuaciones.
  - Construcción de matrices de proyección que relacionan los píxeles con las mediciones de los rayos.
  - Formulación del problema mediante el sistema lineal `Ax = b`.

- **Rango, espacio nulo y unicidad de la reconstrucción:**
  - Estudio del rango y la nulidad de las matrices de proyección.
  - Aplicación de la descomposición en valores singulares (SVD).
  - Construcción de imágenes diferentes que producen las mismas mediciones.

- **Reconstrucción mediante mínimos cuadrados:**
  - Análisis del residuo y del error relativo de reconstrucción.
  - Incorporación de ruido gaussiano a las mediciones y estudio de sus efectos.
  - Interpretación geométrica de mínimos cuadrados mediante proyecciones ortogonales.

- **Métodos de optimización numérica:**
  - Formulación de la función de costo, su gradiente y su Hessiana.
  - Implementación del método de gradiente descendente.
  - Análisis de la tasa de aprendizaje y las condiciones de convergencia.
  - Aplicación del método de Newton 
  - Comparación de los resultados obtenidos mediante mínimos cuadrados, gradiente descendente y Newton.

- **Regularización de imágenes:**
  - Construcción de una matriz de diferencias entre píxeles vecinos.
  - Estudio del efecto del parámetro de regularización `λ` y del nivel de ruido `σ`.
  - Análisis del equilibrio entre el ajuste a las mediciones y la conservación de los detalles de la imagen.

- **Reconstrucción de una imagen de mayor resolución:**
  - Aplicación de los métodos a una imagen desconocida de 128 × 128 píxeles.
  - Reconstrucción mediante gradiente descendente con distintos niveles de regularización.

## Herramientas y tecnologías

- **Lenguaje:** Python.
- **Entorno:** Jupyter Notebook.
- **Bibliotecas principales:**
  - `NumPy`: operaciones matriciales y álgebra lineal.
  - `SciPy`: métodos numéricos, matrices dispersas y cálculo de autovalores.
  - `Matplotlib`: visualización de imágenes, errores y resultados de los algoritmos.

## Organización del repositorio

El desarrollo se encuentra organizado en notebooks de Jupyter, desde `ejercicio_1.ipynb` hasta `ejercicio_11.ipynb`, que abordan progresivamente la construcción del modelo tomográfico, el análisis de sus propiedades matemáticas y la aplicación de distintos métodos de reconstrucción.

## Objetivo del trabajo

Comprender cómo las propiedades de las matrices de proyección, la cantidad de mediciones, el ruido y los métodos de optimización influyen en la reconstrucción de imágenes tomográficas, evaluando las ventajas y limitaciones de cada enfoque.
