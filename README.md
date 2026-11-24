# AeroLista

Proyecto integrador de Estructuras de Datos. Permite reservar, consultar, modificar y cancelar asientos del vuelo AL-204. Flask conecta la interfaz con una lista simplemente enlazada de pasajeros.

## Ejecutar el proyecto

Desde la carpeta del proyecto, crea y activa un entorno virtual.

| Windows (PowerShell) | macOS o Linux |
| --- | --- |
| `py -m venv venv` | `python3 -m venv venv` |
| `.\venv\Scripts\Activate.ps1` | `source venv/bin/activate` |

```bash
python -m pip install -r requirements.txt
python app.py
```

Abre [AeroLista](http://127.0.0.1:5050). El vuelo tiene 68 asientos y la primera ejecución carga 12 reservas de ejemplo.

## Comprobar la entrega

- Ejecuta `python prueba_consola.py` para probar los nueve métodos de la lista enlazada desde la terminal.
- En **Progreso del backend**, pulsa **Revisar otra vez**. El verificador comprueba los nueve métodos, incluidos los distintos casos de eliminación, y el panel debe mostrar **9/9**.
- Al reservar, modificar o cancelar, los cambios se guardan en `data/reservas.json` y se recuperan al reiniciar Flask. El botón **Datos de ejemplo** restaura las 12 reservas originales.
