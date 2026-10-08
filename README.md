# Notas Rápidas (Tkinter)

Mini-app de escritorio para practicar el manejo de eventos de botón, teclado y ratón con Tkinter.

## Dependencias

- Python 3.10 o superior
- Tkinter (viene incluido con Python; en Linux: `sudo apt install python3-tk`)
- No requiere paquetes externos

## Cómo ejecutar

```bash
cd notas_tk
python app.py
```

Al agregar la primera nota se crea el archivo `notas.json` en la misma carpeta que `app.py`.

## Funcionalidades

- Campo de texto y botón **Agregar**
- Lista de notas y botón **Eliminar**
- Contador de notas ("1 nota" / "n notas")
- Editar una nota con doble clic
- Búsqueda: el campo **Buscar** resalta en amarillo las notas que coinciden
- Persistencia: las notas se guardan y se cargan desde `notas.json`
- Tema claro/oscuro con el botón **Tema** (se recuerda al reabrir)

### Eventos manejados

| Evento | Control | Acción |
|---|---|---|
| Clic en botón (`command`) | Agregar | Agrega la nota |
| Clic en botón (`command`) | Eliminar | Elimina la nota seleccionada |
| Clic en botón (`command`) | Tema | Cambia entre tema claro y oscuro |
| Tecla Enter (`<Return>`) | Campo de texto | Agrega la nota |
| Doble clic (`<Double-Button-1>`) | Lista | Edita la nota con un diálogo |
| Escritura (`trace_add("write")`) | Campo de búsqueda | Resalta las notas que coinciden |

## Controles usados

`texto`, `Boton`, `Lista`, `Etiqueta`, `Marco`.

