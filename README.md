# fet-tests

Pruebas de generación de horarios con [FET](https://lalescu.ro/liviu/fet/) (`fet-cl` 7.10.5) para el proyecto Capstone del DISC.

| Cuaderno | Qué hace | Datos que debes subir | Binder |
|---|---|---|---|
| [`fet_demo/fet_demo.ipynb`](fet_demo/fet_demo.ipynb) | Demostración: construye un problema de FET desde una oferta académica y genera un horario | Una oferta académica `.xlsx` (p. ej. `Oferta Académica ICCI 202620.xlsx`) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Capstone-2026-DISC/fet-tests/main?urlpath=lab/tree/fet_demo/fet_demo.ipynb) |
| [`fet_etl_reschedule_export/fet_etl_reschedule_export.ipynb`](fet_etl_reschedule_export/fet_etl_reschedule_export.ipynb) | ETL de la planilla del cliente, varias versiones de horario, replanificación parcial y exportación a Excel/CSV | `datos cliente.xlsx` (planilla del Encargado Docente) | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/Capstone-2026-DISC/fet-tests/main?urlpath=lab/tree/fet_etl_reschedule_export/fet_etl_reschedule_export.ipynb) |

## Los datos no están en este repositorio

Las planillas reales contienen RUT y nombres de personas, por lo que **no se versionan** (el `.gitignore` excluye `*.xlsx`). Al ejecutar un cuaderno sin el archivo, la celda de carga muestra un botón **Subir .xlsx**; también puedes arrastrar el archivo al panel de archivos de JupyterLab, dentro de la carpeta del cuaderno, y volver a ejecutar esa celda. En Google Colab se abre el selector de subida. Los archivos subidos viven solo en la sesión y se pierden al cerrarla.

## Ejecución

- **Binder:** usa los botones de la tabla. La primera vez descarga `fet-cl` (binario con Qt incluido).
- **Local:** `pip install -r binder/requirements.txt` y `jupyter lab`; deja el `.xlsx` junto al cuaderno.
- **Colab:** abre el `.ipynb` desde GitHub y sube el `.xlsx` cuando se pida.

Licencia: AGPL-3.0 (ver `LICENSE`).
