# Comparador de Escalas: Lineal vs Logarítmica

![Licencia](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-blue.svg)
![Version](https://img.shields.io/badge/version-1.0.0-green)
![Tech](https://img.shields.io/badge/Tech-JavaScript%20|%20SVG%20|%20MathJax-orange)

Una herramienta interactiva y con fines educativos diseñada para visualizar y comprender las diferencias fundamentales entre las **escalas lineales** y las **escalas logarítmicas**. Ideal para entornos educativos, científicos y de análisis de datos.


## Características Principales

* **Comparador Visual:** Visualiza cómo se distribuyen los mismos puntos de datos en ambos tipos de escalas simultáneamente.
* **Valor Dinámico Interactivo:** Incluye un slider para observar el desplazamiento proporcional y cómo la escala logarítmica "comprime" los órdenes de magnitud.
* **Calculadora de Logaritmos:** Soporta bases personalizadas ($b$) y argumentos ($x$), con renderizado matemático elegante mediante **MathJax**.
* **Diseño Responsivo:** Interfaz optimizada para escritorio y dispositivos móviles con un estilo moderno .
* **Algoritmos de Visualización "Nice Number":** Implementa lógica avanzada para generar ejes con marcas (ticks) redondas y legibles, similar a librerías de alto nivel como D3.js.

---

## Tecnologías Utilizadas

* **HTML5 & CSS3:** Estructura semántica y diseño basado en variables CSS (Custom Properties).
* **Vanilla JavaScript (ES6+):** Arquitectura basada en el patrón de diseño **IIFE** (Immediately Invoked Function Expression) para encapsulamiento y robustez.
* **SVG (Scalable Vector Graphics):** Generación dinámica de gráficos para una nitidez absoluta en cualquier resolución.
* **MathJax 3:** Renderizado de fórmulas matemáticas en alta calidad.
* **Google Fonts:** Tipografía "Inter" para máxima legibilidad.

---

## Conceptos Matemáticos Aplicados

### Transformación Logarítmica
El corazón de la aplicación es el mapeo de valores a coordenadas de píxeles. Mientras que en la escala lineal la posición es proporcional al valor, en la logarítmica la posición es proporcional al exponente:

$$x_{pixel} = offset + \left( \frac{\log_{10}(x) - \log_{10}(x_{min})}{\log_{10}(x_{max}) - \log_{10}(x_{min})} \right) \cdot width$$

Esto permite que la distancia visual entre $1$ y $10$ sea idéntica a la distancia entre $10$ y $100$.

---

## Instalación y Uso

No requiere dependencias externas ni compilación. 

[1. Clona el repositorio:](https://saintunderman.github.io/matematica_santiago_fiore_simulador_conversor_de_escalas/)
   ```bash
   git clone [https://github.com/tu-usuario/nombre-del-repo.git](https://github.com/tu-usuario/nombre-del-repo.git)
