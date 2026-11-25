# Modelos Discretos: Exponencial y Logístico

Proyecto desarrollado en **Python** para el curso de **Modelamiento Matemático**, enfocado en el modelado, simulación y análisis de sistemas dinámicos en tiempo discreto mediante los modelos exponencial y logístico.

## Fundamento de los modelos

### Modelo exponencial discreto
Describe un crecimiento o decrecimiento proporcional al tamaño actual de la población o variable en cada paso de tiempo $n$:

$$x_{n+1} = r \, x_n$$

donde $x_n$ es el valor en el paso $n$ y $r$ es el factor de crecimiento por iteración.

### Modelo logístico discreto
Incorpora un límite de saturación o capacidad de carga ($K$) que frena el crecimiento a medida que el sistema se acerca a su valor máximo:

$$x_{n+1} = x_n + r_d \, x_n \left(1 - \frac{x_n}{K}\right)$$

(o en su forma normalizada $x_{n+1} = \mu \, x_n (1 - x_n)$), permitiendo observar convergencia al equilibrio, oscilaciones o comportamiento caótico según el parámetro de crecimiento.

## Contenido del repositorio

* Cuaderno de Jupyter / scripts con la implementación iterativa de ambos modelos, ajuste o evaluación de parámetros, simulación de trayectorias y gráficas comparativas.
* `.gitignore`: Exclusión de archivos temporales, caché y entornos virtuales.

## Herramientas utilizadas

* **Python 3** y **Jupyter Notebook**
* **NumPy** (cálculo numérico y simulación discreta)
* **Matplotlib** (visualización de trayectorias y comparación de modelos)
