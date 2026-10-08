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
- Tema claro/oscuro con el botón **Tema** 

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

`texto`, `Boton`, `Lista`, `Etiqueta`.


## Capturas de pantalla

Agrega aquí tus capturas de la app en ejecución:

1. Tema claro con varias notas
   <img width="2262" height="1302" alt="imagen" src="https://github.com/user-attachments/assets/e7c2fe4f-933d-4243-aeb1-43767251a8bc" />

3. Tema oscuro
   <img width="2377" height="1327" alt="imagen" src="https://github.com/user-attachments/assets/7fadade8-69da-463f-aa6c-454d9ef485a1" />

5. Búsqueda con notas resaltadas
   <img width="1927" height="1256" alt="imagen" src="https://github.com/user-attachments/assets/5d7603d1-b365-4f2d-8e96-f1bcce74ef5e" />

7. Diálogo de edición
   
   Aqui le apretamos doble click a la nota que queramos editar, en este caso fue la de ¨Pendientes 2¨
   <img width="2037" height="1250" alt="imagen" src="https://github.com/user-attachments/assets/edf51ad2-39ed-4d1b-b782-ac4ba89bc983" />

   Aqui cambiamos el nombre al que queramos en este caso fue ¨Pendientes 3¨ y luego le damos ¨OK¨ para guardar, y vemos que ya se edito
   <img width="1997" height="1308" alt="imagen" src="https://github.com/user-attachments/assets/9e5dbeda-bd0d-46e6-ab27-1e30cf2b2cc0" />

   
   

