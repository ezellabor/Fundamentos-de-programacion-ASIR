# Práctica 2 – Siguiendo el rastro de las variables  
**Unidad 1** – Identificadores, Variables y Constantes  
**Módulo:** Fundamentos de Programación | ASIR1  
**Descripción:** Uso del depurador (modo paso a paso) en PSeInt para observar la evolución de variables y constantes

**Profesor:** Ezequiel Llarena Borges  

---

## Qué se espera que logres al finalizar la práctica

### Resultados de aprendizaje
- RA1: Reconocer la ejecución secuencial de instrucciones y la evolución del estado de las variables.  
- RA2: Comprender la utilidad del depurador para analizar y corregir programas.

### Criterios de evaluación
- CE1.1: Usa correctamente el modo “Depurar” o “Paso a paso” de PSeInt.  
- CE1.2: Interpreta los cambios de valores en las variables durante la ejecución.  
- CE1.3: Corrige errores simples observando el comportamiento de las variables.

---

## Objetivos de la unidad
- Aprender a ejecutar un algoritmo paso a paso en PSeInt.  
- Observar cómo cambian las variables en cada instrucción.  
- Entender la diferencia entre **valor inicial, intermedio y final** de una variable.  
- Usar el depurador como herramienta para detectar errores lógicos.

---

## Parte 1 – Preparación del entorno

> **Nota:** Esta sección sirve para preparar el entorno de trabajo.

1. Abre **PSeInt** y asegúrate de que la vista *Panel de variables* está visible.  
   - Si no la ves, actívala en el menú: `Ver → Panel de seguimiento`.  
2. Crea un nuevo algoritmo llamado `Depuracion_Variables`.  
3. Copia este código inicial:

```pseudocode
Algoritmo Depuracion_Variables
   Definir edad, aumento Como Entero
   Definir nombre Como Cadena
   Definir sueldo, nuevoSueldo Como Real
   Const IVA <- 0.21

   nombre <- "Alex"
   edad <- 20
   sueldo <- 1200
   aumento <- 100

   nuevoSueldo <- sueldo + aumento
   Escribir "Empleado: ", nombre
   Escribir "Edad: ", edad
   Escribir "Sueldo con aumento: ", nuevoSueldo

   Escribir "Sueldo con IVA: ", nuevoSueldo * (1 + IVA)
FinAlgoritmo
