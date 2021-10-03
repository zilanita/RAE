# Todas las definiciones de la RAE en .txt
Las palabras se extrajeron del trabajo de: https://github.com/JorgeDuenasLerin/diccionario-espanol-txt

Puede llegar y tomar los .txt y usarlos puesto que ya están pulidos. Si quiere saber sobre el método de extracción lea lo que sigue.

Extraídos con Selenium-Python.

El código está en Python_Selenium_code.txt y usa Google Chrome.

Para usarlo debe ingresar este código en Python (luego de hacer los enlaces con Selenium) y hacer las modificaciones del código de forma que usted cree dos .txt:
  - Uno que contenga las palabras que desea buscar en la RAE (separadas por un salto de línea).
  - Otro en el cual se registrarán las definiciones en formato lista C++.


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

Pese a esto, lo subí puesto que nadie (al parecer) lo había hecho de manera expedita en .txt. Ojalá que a alguien le sirva ;)
