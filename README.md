# Restaurante App - Semana 14

## Estudiante
Milton Paul Guachala Quinatoa

## Descripción

En esta semana continué el proyecto `restaurante_app` de la Semana 13. La idea fue mejorar la interfaz que ya tenía y aplicar componentes y contenedores de Tkinter/ttk de una forma más ordenada.

Ahora la aplicación tiene un menú lateral, formularios, botones de acción y tablas para consultar la información. En Productos se pueden registrar, consultar, actualizar y eliminar productos, y los cambios se guardan en `productos.json` mediante `RestauranteServicio`.

## Estructura

```text
restaurante_app/
├── datos/
│   ├── productos.json
│   └── usuarios.json
├── modelos/
│   ├── __init__.py
│   ├── producto.py
│   └── usuario.py
├── servicios/
│   ├── __init__.py
│   ├── archivo_servicio.py
│   └── restaurante_servicio.py
├── ui/
│   ├── __init__.py
│   ├── login_view.py
│   └── main_view.py
├── assets/
│   ├── icons/
│   └── logo/
└── main.py
```

## Componentes y contenedores utilizados

Se utilizaron `Frame` y `LabelFrame` para separar las diferentes zonas de la aplicación. También se utilizaron `Label`, `Entry`, `Button`, `Treeview` y `Scrollbar` para capturar y mostrar la información.

Los gestores de geometría usados son principalmente `pack()`, `grid()` y `place()`, según la necesidad de cada parte de la interfaz.

## Funcionalidades

- Inicio de sesión con validación mediante `RestauranteServicio`.
- Consulta de usuarios registrados.
- Consulta de productos.
- Registro de productos.
- Carga o consulta de un producto por código.
- Actualización de productos.
- Eliminación de productos.
- Actualización de las tablas después de cada operación.
- Persistencia de productos mediante `productos.json`.
- Cierre de sesión.
- Se mantiene Ventas como funcionalidad pendiente.

## Separación de responsabilidades

La interfaz se encarga de mostrar la información y recibir los datos. `RestauranteServicio` realiza las operaciones sobre los productos y sus validaciones, mientras que `ArchivoServicio` se encarga de leer y escribir los archivos JSON.

## Credenciales de demostración

Usuario | Contraseña

`Milton` `admin` 
`Sofia` `sofia123`
`Carlos` `carlos123`
`Valentina` `vale123`
`Diego` `diego123`
`Camila` `camila123`
`Andres` `andres123`
`Gabriela` `gabi123`

## Cómo ejecutar

Desde la carpeta `restaurante_app` ejecutar:

```bash
python main.py
```

También se puede ejecutar desde VS Code con **Run Python File**.

