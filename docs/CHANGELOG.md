# Changelog

Todos los cambios relevantes de este proyecto se documentan en este archivo.
El formato sigue [Keep a Changelog](https://keepachangelog.com/es-ES/1.1.0/) y el versionado es [SemVer](https://semver.org/lang/es/).

## [Sin publicar]

### Ideas para próximas versiones
- Calcular el próximo `idPartida` leyendo el último registro del archivo, para que los IDs no se reinicien en cada ejecución.
- Validar la opción de jugada (1-3) y la entrada no numérica.
- Evitar que una coma en el nombre del jugador corrompa el formato CSV.
- Agregar estadísticas (victorias, derrotas y empates).

## [1.0.0] - 2026-10-12

### Agregado
- Estructura `Partida` con ID, jugador, elección del jugador, elección de la IA y resultado.
- Menú principal con tres opciones: jugar, ver historial y salir.
- Elección aleatoria de la IA con `rand()` y `srand(time(0))`.
- Evaluación de reglas: Victoria, Derrota y Empate.
- Persistencia en `src/historial_partidas.txt` con `ofstream` en modo `ios::app`.
- Lectura del historial con `ifstream` y despliegue en pantalla.
- Documentación: README, manual de usuario, manual del programador, informe APA v7.
- Archivos de repositorio: `LICENSE` (MIT), `.gitignore` y `.gitattributes`.
