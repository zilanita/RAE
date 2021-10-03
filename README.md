# Todas las definiciones de la RAE en .txt
Las palabras se extrajeron del trabajo de: https://github.com/JorgeDuenasLerin/diccionario-espanol-txt

Puede llegar y tomar los .txt y usarlos puesto que ya están pulidos. Si quiere saber sobre el método de extracción lea lo que sigue.

Extraídos con Selenium-Python.
El código está en Python_Selenium_code.txt y usa Google Chrome.
Para usarlo debe ingresar este código en Python (luego de hacer los enlaces con Selenium) y hacer las modificaciones del código de forma que usted cree dos .txt:
  - Uno que contenga las palabras que desea buscar en la RAE.
  - Otro en el cual se registrarán las definiciones en formato lista C++.
En Dev-C++ se vería algo así:

#include<stdio.h>
#define DEF 62
#define SPACE 698
char palabra[][DEF+2][SPACE+1]={
  /*...*/
  {"ababillarse","1. prnl. rur. Chile. Dicho de un animal: Enfermar de la babilla."},
  {"ababol","1. m. Esp. orient. amapola.","2. m. Ar. y Nav. Persona distraída, simple, abobada."},
  {"abacá","1. m. Planta de la familia de las musáceas, de unos tres metros de altura, originaria de Filipinas, y de cuyo tronco se saca un filamento textil."}
  {"abacal","1. m. Filip. Terreno donde se cultiva abacá."},
  {"abacalera","1. adj. Filip. Perteneciente o relativo al abacá o al abacal."},
  /*...*/
  NULL,
  };

Note que la palabra en sí va en la primera direccion, mientras que las definiciones van en las siguientes.

Pros del código en Python:
  - Fácil de entender pues solo usa ciertos aspectos básicos de Python y Selenium.
Contras:
  - Demasiado lento, tarda días en registrar todas las palabras.
  - Se salta palabras.
  - Se salta definiciones.
  - Puede contener errores.
  - Se interrumpe sin motivo aparente.
  - Si se interrumpe puede generar errores en el texto.
  - No distingue las comillas dentro de una definición, por lo que las palabras:
          dilogía
          bajo
          clicar
          ecuación
        Deben corregirse manualmente antes de introducir el listado en el sketch de Dev-C++
        Sin embargo, esto ya está corregido en los archivos de texto incluidos en el repositorio.
