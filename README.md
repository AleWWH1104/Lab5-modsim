# Laboratorio 5 – Modelación y Simulación

Modelo espacial de cobertura hospitalaria para **Wisconsin (WI)**. Se combinan las geometrías de condados, los hospitales con capacidad de camas, la población por condado y los límites estatales para estimar qué parte de la población tiene un hospital a una distancia razonable y dónde están las brechas. Las instrucciones completas están en `S13 - Laboratorio 5-1.pdf`.

Integrantes: Iris Ayala, Anggie Quezada, Jonathan Diaz

## 1. Crear el entorno

Se necesita [uv](https://docs.astral.sh/uv/) (`brew install uv` o `pip install uv`).

```bash
uv sync
```

## 2. Datos

Los cuatro archivos de Canvas ya están en la carpeta `datos/`, no hay que descargar nada:

- `hospitales_eeuu.geojson`
- `condados_eeuu.geojson`
- `estados_eeuu.geojson`
- `poblacion_condados.csv`

## 3. Correr el notebook

Abrir `Lab5.ipynb` en VS Code o Jupyter (`uv run jupyter lab`), seleccionar el kernel de `.venv` y ejecutar todas las celdas.
