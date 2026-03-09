# Biblioteca - Gestión de Libros

Este es un programa simple en Python que permite gestionar información de libros mediante una clase llamada `Libro`.

## Descripción

La clase `Libro` proporciona funcionalidades básicas para:

- **Crear** un registro de libro con título, autor y número de páginas
- **Mostrar** la información completa del libro
- **Actualizar** el número de páginas con validación

## Estructura de la Clase

### Atributos

| Atributo | Descripción |
|----------|-------------|
| `titulo` | Título del libro |
| `autor` | Autor del libro |
| `numero_paginas` | Número de páginas del libro |

### Métodos

#### `__init__(self, titulo, autor, numero_paginas)`
Constructor que inicializa un nuevo libro con los parámetros proporcionados.

**Parámetros:**
- `titulo` (str): Título del libro
- `autor` (str): Autor del libro
- `numero_paginas` (int): Número de páginas

#### `mostrar_informacion(self)`
Muestra por consola la información completa del libro formateada en un recuadro.

#### `actualizar_paginas(self, nuevo_numero_paginas)`
Actualiza el número de páginas del libro.

**Parámetros:**
- `nuevo_numero_paginas` (int): Nuevo número de páginas

**Validación:** El número de páginas debe ser mayor a 0. Si no cumple, muestra un mensaje de error.

## Ejemplo de Uso

```python
if __name__ == "__main__":
    # Registro de un libro
    libro1 = Libro("Cien Años de Soledad", "Gabriel García Márquez", 417)
    
    # Mostrar la información del libro
    libro1.mostrar_informacion()
    
    # Actualizar el número de páginas
    libro1.actualizar_paginas(422)
```

## Salida Esperada

```
========================================
INFORMACIÓN DEL LIBRO
========================================
Título: Cien Años de Soledad
Autor: Gabriel García Márquez
Número de páginas: 417
========================================
El número de páginas ha sido actualizado a: 422
```

## Requisitos

- Python 3.x

## Cómo Ejecutar

```bash
python Biblioteca.py
```

## Licencia

Este es un proyecto educativo de ejemplo.

