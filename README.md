# Juego de Colocación y Movimiento de Fichas

Este programa permite cargar un nivel desde un archivo de texto y jugar un juego de colocación y movimiento de fichas sobre un tablero. Las fichas pueden rotarse, voltearse, colocarse en el tablero y moverse dentro de él según ciertas reglas.

## Características del Juego
- Carga un tablero desde un archivo de texto.
- Permite la selección de fichas y su manipulación (rotación y volteo).
- Posibilidad de colocar fichas en el tablero en una posición determinada.
- Movimiento de fichas ya colocadas respetando restricciones.
- Eliminación de fichas del tablero.
- Verificación de victoria cuando el tablero está completamente lleno.

## Requisitos
- Python 3.x

## Instrucciones de Uso
1. Ejecutar el script `python nombre_del_script.py`.
2. Seleccionar un nivel entre 1 y 3.
3. Visualizar el tablero y las fichas disponibles.
4. Interactuar con el juego mediante las opciones:
   - **1:** Modificar la orientación de una ficha (rotación o volteo).
   - **2:** Añadir una ficha al tablero.
   - **3:** Mover una ficha ya colocada en el tablero.
   - **4:** Eliminar una ficha del tablero.
5. Continuar hasta llenar el tablero completamente o salir del juego.

## Formato del Archivo de Nivel
Cada archivo de nivel sigue la estructura:
```
<filas> <columnas>
<matriz del tablero con 0 para espacio vacío y 1 para ocupable>
<numero de fichas>
<dimensiones de ficha 1>
<matriz de ficha 1 con 0 para espacio vacío y 1 para parte de la ficha>
...
<dimensiones de ficha N>
<matriz de ficha N>
```

## Funciones Principales
### `cargar_nivel(archivo)`
Carga el tablero y las fichas desde un archivo de nivel.

### `imprimir_tablero(tablero)`
Muestra el estado actual del tablero en la consola.

### `imprimir_fichas(fichas)`
Imprime las fichas disponibles para jugar.

### `rotacion_interactiva(matriz)`
Permite al usuario rotar o voltear una ficha.

### `verificar_pieza(tablero, pieza)`
Verifica si una ficha está en el tablero.

### `coordenadas(tablero, pieza, fichas)`
Obtiene las coordenadas de una ficha en el tablero o en la lista de fichas.

### `victoria(tablero)`
Verifica si el tablero está completamente lleno.

### `iniciar_juego()`
Controla la lógica principal del juego.

## Notas Adicionales
- Las fichas solo pueden moverse a posiciones con `#`.
- Si una ficha ya está en el tablero, no puede añadirse de nuevo.
- Los movimientos están restringidos por los límites del tablero y otras fichas.

## Autor
Creado por [Tu Nombre].

