# Simulador de Capacidad y Planificación — Caso 2: Segunda Vida

## ¿Quién utilizaría esta herramienta y qué decisión ayuda a tomar?
Esta herramienta está diseñada para la **responsable de campaña (Alicia)**, el **encargado de taller (Bruno)** y la **coordinadora de pedidos (Celia)** de *Segunda Vida*. Permite decidir qué alternativa operativa contratar (**Referencia**, **Opción A: Organizador**, **Opción B: Cuarta persona** o **Opción C: Módulo preparado**) para cumplir con la demanda de mandos reacondicionados y el nivel de calidad exigido al menor coste incremental diario factible.

## Instrucciones de ejecución
1. Descarga o clona este repositorio en tu computadora.
2. Abre el archivo `index.html` haciendo doble clic sobre él en cualquier navegador web moderno (Chrome, Edge, Firefox, Safari).
3. No requiere conexión a internet, instalación de servidores, bases de datos ni claves de API.
4. Ingresa los 5 parámetros del escenario o utiliza el botón **Escenario Base** para restaurar los valores iniciales.

## Qué NO puede afirmar esta herramienta (Límites)
* **No garantiza entregas turno a turno:** Opera con tiempos estándar medios y tasas esperadas deterministas; no modela colas estocásticas ni variabilidad aleatoria entre llegadas.
* **No sustituye estudios de tiempos futuros:** Los parámetros de las opciones A, B y C provienen de pilotos sintéticos de 50 entradas.
* **No evalúa ergonomía ni seguridad:** El cumplimiento de alcances ($\le 32\text{ cm}$) debe verificarse físicamente en el puesto.

## Pruebas de validación incluidas
La aplicación valida entradas inválidas (valores vacíos, negativos, $r \notin [0,1]$, $y_{min} \notin [0,1]$, minutos $\le 0$), escenarios inviables por capacidad o suministro ($N > 300$) y coincide exactamente con las 3 pruebas manuales del punto de control y la extensión de rendimiento $99.5\%$.

## Declaración breve de uso de IA
Se utilizó asistencia de inteligencia artificial para estructurar la interfaz HTML/CSS/JS de la microherramienta, verificar la lógica de validación de entradas y redacción del README. Todas las fórmulas de tiempos estándar, balance de cargas, muestreo del trabajo, criterios ergonómicos y decisiones de ingeniería fueron calculadas, verificadas manualmente y aprobadas por los integrantes del equipo.