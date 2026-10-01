# Laboratorio 5 – Modelación y Simulación

Modelo espacial de cobertura de servicios de salud para **Suiza (CHE)**. Se combinan los límites administrativos de GADM, las instalaciones de salud de healthsites.io y la población de WorldPop para estimar qué parte de la población tiene un servicio de salud a una distancia razonable y dónde están las brechas. Las instrucciones completas están en `S13 - Laboratorio 5.pdf`.

Integrantes: Iris Ayala, Anggie Quezada, Jonathan Diaz

## 1. Crear el entorno

Se necesita [uv](https://docs.astral.sh/uv/) (`brew install uv` o `pip install uv`).

```bash
uv venv
source .venv/bin/activate
uv pip install geopandas pandas numpy matplotlib requests shapely rasterio python-dotenv jupyter ipykernel
```

## 2. API key de healthsites.io

1. Crear una cuenta en https://healthsites.io/map (botón _Sign up_).
2. Iniciar sesión, ir al perfil y llenar el formulario de API en https://healthsites.io/enrollment/form.
3. Esperar a que los administradores aprueben la llave (puede tardar). Mientras no esté aprobada, la API responde `This API key is not active`.
4. Copiar `env.example` a `.env` y pegar la llave:

```bash
cp env.example .env
```

```
HEALTHSITES_API_KEY=tu_llave_aqui
```

## 3. Correr el notebook

Abrir `Lab5.ipynb` en VS Code o Jupyter (`jupyter lab`), seleccionar el kernel de `.venv` y ejecutar todas las celdas. Los datos se descargan solos a la carpeta `datos/`.
