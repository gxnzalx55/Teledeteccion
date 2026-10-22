# Teledetección 2025 · Laboratorio 1

Cuadernos de Jupyter de **Teledetección**: desde los fundamentos de NumPy hasta el procesado de imágenes de satélite (Landsat, WorldView, Sentinel) y su clasificación.

## Contenido

| Carpeta | Tema | Qué se trabaja |
|---|---|---|
| `0_Conf_Incial` | Configuración inicial | Credenciales y perfil de **Sentinel Hub** (`SHConfig`) |
| `1_Intro` | Introducción | NumPy, funciones lambda, lectura y visualización de imágenes |
| `2_Histo` | Histogramas | Histogramas y operaciones de contraste sobre imágenes y bandas RGB de Landsat |
| `3_Filtros` | Filtros | Filtrado espacial con OpenCV sobre imágenes de Barcelona y WorldView (pancromática) |
| `4_Zoom` | Zoom e interpolación | Reescalado de imágenes y composición de bandas RGB |
| `5_ColorYClasificadores` | Color y clasificación | Espacio HSV, **NDVI**, y clasificación no supervisada con **K-Means** (datos de Sentinel Hub) |

Cada carpeta incluye los cuadernos de práctica (`P*-E*`, `Ejercicio-*`), las tareas entregables (`Tarea*`) y las imágenes de ejemplo que usan.

## Requisitos

- Python 3.10 o superior
- Jupyter (JupyterLab o VS Code)
- Librerías: `numpy`, `pandas`, `matplotlib`, `opencv-python`, `scikit-learn`, `sentinelhub`

```bash
pip install numpy pandas matplotlib opencv-python scikit-learn sentinelhub jupyterlab
```

## Puesta en marcha

1. Clona el repositorio y abre la carpeta en Jupyter.
2. Para los cuadernos que descargan datos de satélite (sobre todo `5_ColorYClasificadores`), crea una cuenta en [Sentinel Hub](https://www.sentinel-hub.com/) y obtén un `Client_ID` y un `Client_Secret`.
3. Ejecuta `0_Conf_Incial/Conf-Inicial.ipynb`: te pedirá las credenciales por consola y las guardará en un perfil de configuración. Puedes repetirlo cuando quieras para corregir errores o cambiar de perfil.
4. Ejecuta el resto de cuadernos en orden.

> No subas nunca tus credenciales al repositorio.

## Estructura

```
.
├── 0_Conf_Incial/
├── 1_Intro/
├── 2_Histo/          # incluye RGB/ con las bandas Landsat
├── 3_Filtros/
├── 4_Zoom/           # incluye RGB/ con las bandas Landsat
└── 5_ColorYClasificadores/
```
