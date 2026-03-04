# ⚓ SEA OF CODE — Batalla Naval en Python

> *< Code. Aim. Fire. />*

Juego de **Batalla Naval por consola** desarrollado en Python como proyecto académico para la asignatura de Programación (G02) — Universidad Autónoma de Occidente, 2026.

---

## 🎮 ¿De qué trata?

Tú y la máquina se enfrentan en alta mar. Cada uno esconde **3 barcos** en un tablero de **5×5**. Por turnos se lanzan ataques hasta que alguien hunda los 3 barcos del rival. ¡El primero en lograrlo gana!

---

## 🖥️ Vista previa

```
╔══════════════════════════════════════════════════════╗
║                                                      ║
║        ⚓     S E A   O F  C O D E     ⚓           ║
║                       5×5                            ║
║                                                      ║
╚══════════════════════════════════════════════════════╝

   A   B   C   D   E
1  0   0   0   0   1
2  0   0   0   0   0
3  0   1   0   0   0
4  0   0   0   1   0
5  0   0   0   0   0
```

---

## 🚀 Cómo ejecutar

### Requisitos
- Python 3.7 o superior
- Jupyter Notebook (opcional, para el `.ipynb`)

### Opción 1 — Jupyter Notebook
```bash
jupyter notebook Sea_of_code.ipynb
```
Ejecuta todas las celdas en orden y luego corre la última celda que llama a `main()`.

### Opción 2 — Terminal (si exportas a `.py`)
```bash
python Sea_of_code.py
```

> ⚠️ El juego usa colores ANSI. Se ve mejor en terminales como PowerShell, bash, zsh o la terminal integrada de VS Code.

---

## 🕹️ Instrucciones del juego

### 1. Tablero
- Cuadrícula de **5 filas × 5 columnas**
- Filas: números del **1 al 5**
- Columnas: letras de la **A a la E**
- Ejemplo de coordenada: `3C` = fila 3, columna C

### 2. Fase de despliegue
- Coloca tus **3 barcos** uno por uno ingresando fila y columna
- No puedes repetir posiciones
- La máquina coloca sus barcos en secreto, de forma aleatoria

### 3. Batalla
- Cada ronda: **primero atacas tú**, luego la máquina
- Ingresa las coordenadas de la casilla que quieres atacar
- No puedes atacar dos veces la misma casilla

### 4. Leyenda del tablero

| Símbolo | Significado |
|---------|-------------|
| `0` | Casilla sin explorar |
| `1` | Barco propio en pie |
| `X` | Barco hundido / impacto recibido |
| `-` | Disparo fallido (agua) |

### 5. Fin de la partida
- Gana quien hunda los **3 barcos** del contrincante primero
- Si ambos hunden el tercero en la misma ronda → **¡Empate!**
- Al final se muestran ambos tableros con el resumen completo

---

## 🧩 Estructura del código

El proyecto está organizado en **7 funciones**:

| Función | Descripción |
|--------|-------------|
| `col_a_indice(letra)` | Convierte una letra (A–E) en su índice numérico (0–4) |
| `pedir_coordenadas(mensaje)` | Solicita y valida fila + columna al usuario |
| `imprimir_tablero(tablero, titulo)` | Muestra el tablero con formato visual en consola |
| `barcos_usuario()` | Permite al jugador colocar sus 3 barcos |
| `barcos_bot()` | Coloca aleatoriamente los 3 barcos de la máquina |
| `ataque_bot(barcos_atk_bot, tablero_usuario)` | Gestiona el ataque aleatorio de la máquina |
| `ataque_usu(barcos_atk_usu, tablero_maquina, tablero_visual_bot)` | Gestiona el ataque del jugador |
| `main()` | Función principal: orquesta el flujo completo del juego |

---

## 📁 Archivos del repositorio

```
📦 Proyecto-Sea-of-code
 ┣ 📓 Sea_of_code.ipynb      # Notebook principal con el código completo
 ┗ 📄 README.md             # Este archivo
```

---

## 👥 Equipo — Startup Sea of Code

| Nombre | GitHub |
|--------|--------|
| Nicolás Armero Rosero | [@Nico08ben](https://github.com/Nico08ben) |
| Sara Mesa Lenis | [@saramesal](https://github.com/saramesal)|
| Karen Juliana Dueñas Castro | [@karen11439](https://github.com/karen11439) |
| Santiago Garcia | [@Sant1833](https://github.com/Sant1833) |

---

## 🏫 Información académica

- **Universidad:** Autónoma de Occidente
- **Facultad:** Ingeniería y Ciencias Básicas
- **Programa:** Ingeniería de Datos e Inteligencia Artificial
- **Asignatura:** Programación (G02)
- **Tutor:** Breyner Posso Bautista
- **Fecha:** Febrero – Marzo 2026

---

## 📄 Licencia

Proyecto académico de uso educativo. © 2026 Sea of Code Team — UAO.
