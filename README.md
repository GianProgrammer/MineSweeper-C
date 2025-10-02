# Buscaminas en C (SDL2 + SDL2_ttf)
[![Screenshot](https://i.ibb.co/DPwJ8fC3/Screenshot.png)](https://ibb.co/CpVcMK7x)

## Requisitos
- Compilador GCC (MinGW en Windows, `build-essential` en Linux)
- [SDL2](https://github.com/libsdl-org/SDL/releases) 2.0.22
- [SDL2_ttf](https://github.com/libsdl-org/SDL_ttf/releases) 2.24.0

## Instalación rápida

### Windows (MinGW)
1. Descarga los *Development Libraries* de SDL2 y SDL2_ttf.
2. Descomprime ambas carpetas aquí mismo (quedarán `SDL2-2.0.22/` y `SDL2_ttf-2.24.0/`).
3. Compila:
   ```bash
        gcc src/*.c -I SDL2-2.0.22/include -I SDL2_ttf-2.24.0/include \
       -L SDL2-2.0.22/lib -L SDL2_ttf-2.24.0/lib \
       -lmingw32 -lSDL2main -lSDL2 -lSDL2_ttf -o buscaminas.exe
    ```
4. Copia los DLLs al lado del .exe:
    SDL2-2.0.22/lib/SDL2.dll
    SDL2_ttf-2.24.0/lib/SDL2_ttf.dll

### Linux
    ```bash
        sudo apt install libsdl2-dev libsdl2-ttf-dev
    ```

## Estructura
.
├── celdas.c/.h
├── estadisticas.c/.h
├── menu.c/.h
├── main.c
├── sprite*.h      (cabeceras con arrays de sprites)
├── SDL2-2.0.22/   (no trackeado)
├── SDL2_ttf-2.24.0/ (no trackeado)
└── README.md

## Autor

Gianluca Ferreyra - 2024