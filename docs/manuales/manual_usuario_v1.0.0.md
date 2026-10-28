# Manual del Usuario - Piedra, Papel o Tijera v1.0.0

EEST N°1 de Vicente López - Laboratorio de Programación (LPR) - 5° 3° A-B - 2026

Autor: Lucas Del Pino

## 1. ¿Qué es este programa?

Es un juego de consola en el que jugás a Piedra, Papel o Tijera contra la computadora. Cada partida que jugás queda guardada en un archivo de texto en tu disco, así que podés cerrar el programa y ver el historial más tarde.

## 2. Requisitos

- Windows 10 u 11.
- Compilador g++ (MinGW) instalado y Visual Studio Code con la terminal PowerShell.

## 3. Cómo iniciar el programa

Abrí PowerShell en la carpeta del proyecto (la raíz del repositorio) y ejecutá:

```
g++ -std=c++11 src/main.cpp -o src/piedrapapelotijera.exe
.\src\piedrapapelotijera.exe
```

Siempre ejecutá el programa desde la raíz del repositorio para que el archivo de historial se guarde y se lea desde el lugar correcto.

## 4. Menú principal

Al iniciar se muestra el menú con tres opciones. Escribí el número y presioná Enter.

- 1 - Jugar Partida: comienza una nueva partida.
- 2 - Ver Historial: muestra todas las partidas guardadas en el disco.
- 3 - Salir: cierra el programa.

Si ingresás un número distinto de 1, 2 o 3, el programa muestra un mensaje de error y vuelve a pedir la opción.

## 5. Cómo jugar una partida

1. Elegí la opción 1 del menú.
2. Escribí tu nombre o nickname y presioná Enter.
3. Elegí tu jugada: 1 (Piedra), 2 (Papel) o 3 (Tijera).
4. El programa muestra qué eligió cada uno y el resultado: Victoria, Derrota o Empate.
5. La partida se guarda automáticamente en el disco.

Reglas: la Piedra le gana a la Tijera, el Papel le gana a la Piedra y la Tijera le gana al Papel. Si ambos eligen lo mismo, es un Empate.

## 6. Ver el historial

Elegí la opción 2. El programa lee el archivo y muestra una línea por partida con el número, el jugador, las jugadas y el resultado, y al final el total de registros. Si todavía no jugaste ninguna partida, muestra un aviso indicando que no hay partidas guardadas.

El historial se conserva aunque cierres la consola y vuelvas a abrir el programa.

## 7. Mensajes del programa

- [DISCO] Partida resguardada con éxito: la partida se guardó correctamente.
- [AVISO] Aún no existen partidas guardadas: todavía no hay historial.
- [ERROR] Opción inválida: ingresaste un número fuera del menú.
- [ERROR] No se pudo abrir el archivo: revisá que estés ejecutando el programa desde la raíz del proyecto y que la carpeta src exista.

## 8. Preguntas frecuentes

- Se saltea la pregunta del nombre: esto ocurre si falta la línea cin.ignore() en el código; usá la versión entregada.
- No encuentro el archivo del historial: se crea al jugar la primera partida, dentro de la carpeta src.
- ¿Puedo borrar el historial? Sí, eliminando el archivo historial_partidas.txt.
- Si escribo una jugada fuera de 1 a 3, el programa la toma como Tijera.
