# juegodenaves
🚀 Juego de Naves en Consola (POO en C++)

Actividad 8 — Programación Orientada a Objetos (POO) en C++ Laboratorio de Programación (LPR) — 5.º año 3.º, Grupos A-B E.E.S.T. N.º 1 "Eduardo Ader" — Vicente López Docente: Mansilla Muñoz York Elías

Mostrar imagen Mostrar imagen Mostrar imagen Mostrar imagen

📖 Descripción

Simulador de combate espacial que se ejecuta en la consola de Windows. El jugador controla una nave, esquiva asteroides que caen y los destruye disparando. El proyecto sirve para aplicar los conceptos básicos de POO: clases, objetos, constructores, atributos privados y métodos públicos (encapsulamiento), como evolución del struct visto en la Actividad 7.

🎮 Controles
Tecla	Acción
W	Mover la nave hacia arriba
A	Mover la nave hacia la izquierda
S	Mover la nave hacia abajo
D	Mover la nave hacia la derecha
ESPACIO	Disparar

Las teclas funcionan con mayúsculas o minúsculas (el código aplica tolower()).

Reglas del juego:

La nave comienza con 3 vidas.
Si un asteroide choca con la nave, se pierde una vida.
Si una bala impacta un asteroide, este se destruye y reaparece arriba en una posición aleatoria.
Con 0 vidas el juego termina y se muestra la pantalla de Game Over.
Al iniciar, el programa pide el nombre y apellido del piloto, que se muestra en pantalla (HUD) y sirve para la captura de evidencia.
🧱 Arquitectura (clases)
Clase	Atributos (private)	Métodos (public)
Nave	x, y, vidas	constructor, getX(), getY(), getVidas(), reducirVida(), pintar(), borrar(), mover(char)
Asteroide	x, y	constructor, getX(), getY(), pintar(), borrar(), mover()
Bala	x, y	constructor, getX(), getY(), mover(), fueraDeRango()

Los atributos son privados: desde main() solo se pueden consultar o modificar a través de los métodos públicos.

⚙️ Requisitos
Sistema operativo: Windows (el código usa windows.h y conio.h).
Compilador: g++ (MinGW-w64 GCC v8.1.0 o superior), estándar C++11.
IDE recomendado: Visual Studio Code con la extensión C/C++ Extension Pack.
Terminal: Windows PowerShell 5.1 o PowerShell Core 7+.
🛠️ Compilación y ejecución

Desde la raíz del proyecto (juegodenaves/), en PowerShell:

powershell
# Compilar
g++ src/main.cpp -o src/juegodenaves.exe

# Ejecutar
.\src\juegodenaves.exe
🗂️ Estructura del repositorio
text
juegodenaves/
├── .gitignore            <-- Exclusiones (.exe, *.out, .vscode/)
├── LICENSE               <-- Licencia MIT escolar
├── README.md             <-- Portada del proyecto
├── docs/                 <-- Documentación formal
│   ├── InformeEEST1_LPR2026_ACT08_G03_v1.0.0.pdf   <-- Informe APA v7
│   ├── CHANGELOG.md                                <-- Historial de versiones
│   └── manuales/
│       ├── manual_programador_v1.0.0.pdf           <-- Manual técnico
│       └── manual_usuario_v1.0.0.pdf               <-- Guía de uso
├── src/                  <-- Código fuente C++
│   └── main.cpp
└── capturas/             <-- Evidencias de ejecución (.png)
    └── combate_consola.png
✨ Funcionalidad extra elegida

(Completar: indicar cuál de las 15 funcionalidades del anexo se implementó y en qué partes de main.cpp se integró.)

📚 Documentación
Manual del programador
Manual de usuario
Informe APA v7
Changelog
🔗 Referencias técnicas
cplusplus.com — Clases y objetos en C++
GeeksforGeeks — Modificadores de acceso en C++
Microsoft Learn — Constructores e inicialización de clases
Git Documentation — Flujo básico y manejo de repositorio

Federico Mattia / Maximo Orue / Ulises Ferrari / Lucas delPino — Estudiantes de 5° 3° año 2026 , E.E.S.T. N.º 1 "Eduardo Ader".
