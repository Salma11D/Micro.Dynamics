# Micro.Dynamics
Dinámica en ciencias económicas

RonDynamicS
Nombre de los integrantes: Ronaldo Batalla Salma Ramadan

Correos institucionales y repositorios: Ronaldo: rbatallaarroyfl@flacso.edu.ec

Repositorio Github: https://github.com/REBA1996/proyecto-sistemas

Salma: sramadanfl@flacso.edu.ec

Repositorio Github:https://github.com/Salma11D/Micro.Dynamics





Se elabora un programa para analizar ecuaciones diferenciales. Este programa proporciona el cálculo de vectores y valores propios asociados a una matriz dada. Además, grafica la dinámica del sistema para comprender sus trayectorias.

Nombre asignado para el programa: Ron´DynamicS , en honor a sus creadores: Ronaldo y Salma

Descripción y explicación del programa elaborado

Este código crea un programa interactivo en Python para trabajar con matrices, resolver sistemas de ecuaciones lineales y analizar sus propiedades, como valores y vectores propios. A continuación una breve explicación de los pasos a seguir para la creación de este programa

Importación de Librerías:

NumPy (np): Para operaciones numéricas 

SymPy (sp): Para matemáticas simbólicas 

ipywidgets: Para crear widgets interactivos 

IPython.display: Para mostrar elementos interactivos

Matplotlib (plt): Para graficar diagramas de fase y soluciones de ecuaciones diferenciales.

SciPy.integrate: Para resolver ecuaciones diferenciales numéricamente.



Función crear_matriz_interactiva(filas, columnas):
Esto nos permite crear crear una matriz de ceros con las dimensiones especificadas por el usuario. Utiliza bucles for y widgets FloatText para generar cuadros de texto donde el usuario puede ingresar los valores de cada elemento de la matriz.

Función confirmar_valores(b):
Recopila los valores ingresados por el usuario en los widgets y los guarda en la matriz. Limpia la pantalla (clear_output) y muestra la matriz ingresada usando sp.Matrix (para una representación formateada).

Función mostrar_ecuaciones(matriz):
Convierte la matriz en un sistema de ecuaciones lineales. Utiliza sp.symbols para crear variables simbólicas (x1, x2, ...). Construye las ecuaciones lineales multiplicando los elementos de la matriz por las variables correspondientes.

Función calcular_valores_vectores_propios(matriz):
Intenta calcular los valores y vectores propios de la matriz usando np.linalg.eig. Muestra los valores y vectores propios calculados numéricamente. Si la matriz no es cuadrada, muestra un mensaje de error.

Función graficar_diagrama_fase(matriz):
Crea un diagrama de fase que visualiza el comportamiento del sistema dinámico definido por la matriz. Utiliza np.meshgrid para crear una malla de puntos en el plano. Calcula las derivadas del sistema (dXdt) usando la matriz y la malla de puntos. Utiliza plt.quiver para dibujar flechas que representan la dirección y magnitud del campo vectorial en cada punto.

Función graficar_solucion_diferencial(matriz):
Resuelve numéricamente la ecuación diferencial 

Función main():
Crea widgets interactivos para que el usuario ingrese las dimensiones de la matriz Muestra un mensaje de error si las dimensiones ingresadas no son válidas.




En resumen, este código proporciona una herramienta interactiva para:

Introducir una matriz cuadrada. Visualizar el sistema de ecuaciones lineales asociado. Calcular y mostrar los valores y vectores propios de la matriz. Visualizar el diagrama de fase del sistema dinámico. Graficar la solución de la ecuación diferencial a través del tiempo.

Fuentes de información
Para la elaboración del programa, no se basó en una única fuente, sino en la integración de conceptos y técnicas de diferentes fuentes de información.

Se utilizaron conceptos fundamentales como matrices, vectores, valores y vectores propios, sistemas de ecuaciones lineales y determinantes. Gilbert Strang, David C. Lay y Serge Lang Ecuaciones diferenciales: Strogatz Steven "nonlinear dynamics and chaos" Ecuaciones Diferenciales con Aplicaciones" de Dennis G.
