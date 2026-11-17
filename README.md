# Nieves 2048
# Capturas de las pruebas

## Ronda 1: Compactar una fila

Rojo: falla porque `motor_2048.dart` no existe.

![R1 rojo](assets/R1_01_rojo_compactar_fila.png)

Verde: `compactarFila` quita los huecos y mantiene el orden.

![R1 verde](assets/R1_02_verde_compactar_fila.png)

## Ronda 2: Fusionar pares adyacentes iguales

Rojo: falla porque `fusionarFila` no existe.

![R2 rojo](assets/R2_01_rojo_fusionar_fila.png)

Verde: `fusionarFila` fusiona pares, sin fusionar tres iguales más de una vez.

![R2 verde](assets/R2_02_verde_fusionar_fila.png)

## Ronda 3: Mover una fila hacia la izquierda

Rojo: falla porque `moverFilaIzquierda` no existe.

![R3 rojo](assets/R3_01_rojo_mover_fila.png)

Verde: orquesta compactar, fusionar y compactar, y reporta si hubo movimiento.

![R3 verde](assets/R3_02_verde_mover_fila.png)

## Ronda 4: Mover la cuadrícula hacia la izquierda

Rojo: falla porque `grid.dart` no existe.

![R4 rojo](assets/R4_01_rojo_grid_izquierda.png)

Verde: `Grid.moverIzquierda` aplica el movimiento a las 4 filas.

![R4 verde](assets/R4_02_verde_grid_izquierda.png)

## Ronda 5: Mover hacia la derecha

Rojo: falla porque `moverDerecha` no existe.

![R5 rojo](assets/R5_01_rojo_grid_derecha.png)

Verde: invierte la fila, reutiliza `moverFilaIzquierda` y vuelve a invertir.

![R5 verde](assets/R5_02_verde_grid_derecha.png)

## Ronda 6: Mover arriba y abajo

Rojo: fallan `moverArriba` y `moverAbajo`.

![R6 rojo](assets/R6_01_rojo_grid_vertical.png)

Verde: se transpone la cuadrícula para reutilizar la lógica horizontal.

![R6 verde](assets/R6_02_verde_grid_vertical.png)

## Ronda 7: Ficha nueva al azar

Rojo: falla porque `agregarFichaAleatoria` no existe.

![R7 rojo](assets/R7_01_rojo_ficha_aleatoria.png)

Verde: se inyecta un `Random` para poder probarlo de forma determinista.

![R7 verde](assets/R7_02_verde_ficha_aleatoria.png)

## Ronda 8: Detectar si quedan movimientos

Rojo: falla porque `hayMovimientosPosibles` no existe.

![R8 rojo](assets/R8_01_rojo_movimientos_posibles.png)

Verde: revisa celdas vacías y vecinos iguales horizontales y verticales.

![R8 verde](assets/R8_02_verde_movimientos_posibles.png)

## Ronda 9: Detectar la victoria

Rojo: falla porque `haGanado` no existe.

![R9 rojo](assets/R9_01_rojo_victoria.png)

Verde: `haGanado` detecta una celda con el valor objetivo.

![R9 verde](assets/R9_02_verde_victoria.png)

## Ronda 10: MotorJuego

Rojo: fallan las pruebas porque `MotorJuego`, `Direccion` y `EstadoJuego` no existen.

![R10 rojo](assets/R10_01_rojo_motor_juego.png)

Verde: `MotorJuego` integra puntaje, turnos, victoria y derrota.

![Todas las pruebas](assets/R10_03_todas_las_pruebas.png)

---

## Interfaz de la aplicacion

![Todas las pruebas](assets/nieves.png)
