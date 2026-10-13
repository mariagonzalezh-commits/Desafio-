# Desafío: Manipulación y Visualización de Datos

Proyecto de la asignatura Estructura de Datos (Corte II), Ingeniería Biomédica.
Profesor: Oscar Stiven Morales Zapata.

Integrantes: Jesica Arango y Maria Fernanda Gonzalez

## Objetivo
Analizar cómo varía el peso corporal de los pingüinos según su especie y su isla, y determinar si el largo de la aleta se relaciona con el peso.

## Datos
- Fuente:dataset de pingüinos de Kaggle (`desafiopinguinos.csv`, separado por `;`).
- Muestra usada: 85 pingüinos elegidos al azar (`random_state=42`) después de eliminar filas con datos vacíos.
- Adaptación: el dataset no tiene columna de eventos ni de año, así que la "cantidad de eventos" es el número de pingüinos por isla y el filtro por año se reemplazó por un filtro por peso.

## Variables principales
| Variable | Descripción |
| --- | --- |
| `species` | Especie del pingüino (Adelie, Chinstrap, Gentoo) |
| `island` | Isla donde vive (Biscoe, Dream, Torgersen) |
| `flipper_length_mm` | Largo de la aleta en milímetros |
| `body_mass_g` | Peso en gramos |

## Qué se hizo
- Lectura del CSV con pandas y limpieza de datos vacíos.
- Cálculo de promedio y desviación estándar del peso.
- Conteo de pingüinos por isla.
- Filtros de datos.
- Peso promedio por especie y correlación entre aleta y peso.
- Gráficos con Matplotlib: histograma, barras y dispersión.
- Exportación de la muestra a Excel (`pinguinos_muestra.xlsx`).

## Archivos del repositorio
| Archivo | Contenido |
| --- | --- |
| `desafiojessymafe.ipynb` | Notebook con todo el código, comentado |
| `desafiopinguinos.csv` | Datos originales |
| `pinguinos_muestra.xlsx` | Muestra de 85 pingüinos exportada |
| `histograma_peso.png`, `barras_isla.png`, `dispersion_aleta_peso.png` | Gráficos |

## Cómo ejecutarlo
1. Clonar el repositorio.
2. Abrir `desafiojessymafe.ipynb` en VS Code.
3. Elegir un kernel de Python con pandas, matplotlib y openpyxl instalados.
4. Ejecutar Restart y Run All.