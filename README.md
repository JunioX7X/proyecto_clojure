# Análisis de Texto en Clojure

Este proyecto contiene funciones para analizar textos en Clojure, dividido en dos módulos principales: `parte1` (análisis de letras) y `parte2` (análisis de palabras y oraciones).

## Módulo `parte1.clj`

### Funciones

1. **`cuentaLetras`**  
   Cuenta la frecuencia de cada letra en un texto (solo letras presentes).  
   - **Ejemplo de salida:** `((\a 10) (\b 5) ...)`  

2. **`cuentaLetras-todas`**  
   Cuenta la frecuencia de todas las letras del abecedario, incluyendo las que no aparecen (frecuencia 0).  
   - **Ejemplo de salida:** `((\a 10) (\b 5) ... (\z 0))`  

## Módulo `parte2.clj`

### Funciones

1. **`conteo-palabras`**  
   Devuelve el número total de palabras en el texto.  

2. **`palabras-unicas`**  
   Retorna una lista ordenada alfabéticamente de palabras únicas (sin repetir).  

3. **`frecuencia-palabras`**  
   Muestra las 10 palabras más frecuentes en el texto, ordenadas por frecuencia descendente.  

4. **`promedio-longitud`**  
   Calcula la longitud promedio de las palabras en el texto.  

5. **`cantidad-oraciones`**  
   Cuenta el número de oraciones (separadas por `.`, `!` o `?`).  

6. **`top-palabras-largas`**  
   Devuelve las 5 palabras más largas del texto.  

7. **`histograma-longitud`**  
   Genera un histograma de frecuencias de longitudes de palabras.  

8. **`oraciones-con-patron`**  
   Filtra oraciones que contienen un patrón específico (ignorando mayúsculas/minúsculas).  

## Ejemplo de Uso

El archivo `prueba.clj` contiene un ejemplo de ejecución con un texto de prueba. Para ejecutarlo, usa:

```clojure
(require '[prueba :as p])
