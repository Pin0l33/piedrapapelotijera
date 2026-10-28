# Piedra, Papel o Tijera con persistencia de datos

Actividad 7 de Laboratorio de Programacion (LPR) - 5° 3° A-B - EEST N°1 de Vicente Lopez - 2026

Mini juego de consola en C++ contra la IA. Cada partida se guarda en una estructura (`struct Partida`) y se persiste en un archivo de texto (`historial_partidas.txt`) usando `fstream` (`ofstream` con `ios::app` e `ifstream`).

## Integrantes

- Lucas Del Pino (5° 3° A-B)

Docentes: Prof. Mansilla Munoz York, Prof. Yamil De Jesus Ganduglia

## Estructura del repositorio

```
piedrapapelotijera/
├── .gitattributes
├── .gitignore
├── LICENSE
├── README.md
├── CHANGELOG.md
├── docs/
│   ├── InformeEEST1_LPR2026_ACT07_G03_DelPinoLucas_Informe_v1.0.0.pdf
│   └── manuales/
│       ├── manual_programador_v1.0.0.md / .pdf
│       └── manual_usuario_v1.0.0.md / .pdf
├── src/
│   └── main.cpp
├── data/
│   └── historial_partidas.txt   (archivo de persistencia)
└── capturas/
    ├── jugada_consola.png
    └── archivo_disco.png
```

## Compilar y ejecutar (PowerShell, Windows 10/11)

```
g++ -std=c++11 src/main.cpp -o src/piedrapapelotijera.exe
.\src\piedrapapelotijera.exe
```

Ejecutar siempre desde la raiz del repositorio.

## Persistencia

El programa crea el archivo `historial_partidas.txt` la primera vez que se juega una partida. Segun la ruta del codigo (`src/historial_partidas.txt`) se genera dentro de `src/`; para la entrega, copiar ese archivo a `data/`.

## Documentacion

- Informe APA v7: `docs/`
- Manual del programador: `docs/manuales/manual_programador_v1.0.0.pdf`
- Manual del usuario: `docs/manuales/manual_usuario_v1.0.0.pdf`
- Historial de versiones: `CHANGELOG.md`

## Licencia

MIT (ver `LICENSE`).
