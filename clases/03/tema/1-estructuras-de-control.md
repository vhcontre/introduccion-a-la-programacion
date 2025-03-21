# **📌 Estructuras de Control**  

## 🖥️ **Estructuras de Control**  
📌 Permiten modificar el flujo de ejecución de un programa, rompiendo la secuencialidad normal.  
📌 Se dividen en **estructuras de decisión** y **estructuras iterativas**.  

---

### **🧩 1. Algoritmos Lineales**  
✔️ Son algoritmos que se ejecutan en orden secuencial, sin tomar decisiones ni repetir acciones.  
✔️ Se ejecutan de arriba hacia abajo, instrucción por instrucción.  

Ejemplo:  
```python
a = 10
b = 20
suma = a + b
print(suma)  # Se ejecuta sin condiciones ni repeticiones
```

---

### **🛑 2. Ruptura de la Secuencialidad**  
📌 Ocurre cuando se introduce una **estructura de control** que altera el flujo normal del programa.  
📌 Se produce en dos casos:  
   - **Decisiones** (cuando hay condiciones que determinan el flujo).  
   - **Iteraciones** (cuando se repiten acciones según una condición).  

---

## **🔹 3. Estructuras de Decisión**  
📌 Permiten que un programa tome decisiones basadas en condiciones.  

### **📍 Decisión Simple (if)**  
✔️ Ejecuta un bloque de código solo si se cumple una condición.  

Ejemplo en Python:  
```python
edad = 18
if edad >= 18:
    print("Eres mayor de edad")
```

---

### **📍 Decisiones Anidadas (if dentro de if)**  
✔️ Se utilizan cuando una condición depende de otra.  

Ejemplo en Python:  
```python
edad = 18
if edad >= 18:
    if edad >= 65:
        print("Eres adulto mayor")
    else:
        print("Eres adulto joven")
```

---

### **📍 Decisión Múltiple (if - elif - else / switch-case en otros lenguajes)**  
✔️ Permite evaluar múltiples condiciones.  

Ejemplo en Python:  
```python
dia = "lunes"

if dia == "lunes":
    print("Inicio de semana")
elif dia == "viernes":
    print("Fin de semana")
else:
    print("Día intermedio")
```

---

## **🔁 4. Estructuras Iterativas (Bucles)**  
📌 Permiten repetir un bloque de código mientras se cumpla una condición.  

---

### **📍 "Repetir-Mientras" (do-while en otros lenguajes)**  
✔️ Ejecuta el bloque de código **al menos una vez**, luego evalúa la condición.  
✔️ No existe en Python, pero se puede simular con un `while`.  

Ejemplo en Python:  
```python
while True:
    num = int(input("Ingresa un número mayor a 0: "))
    if num > 0:
        break
```

---

### **📍 "Mientras-Hacer" (while en Python)**  
✔️ Repite el bloque **mientras la condición sea verdadera**.  

Ejemplo en Python:  
```python
contador = 1
while contador <= 5:
    print("Iteración", contador)
    contador += 1
```

---

### **📍 "Para-Hacer" (for en Python)**  
✔️ Itera una cantidad específica de veces sobre una secuencia.  

Ejemplo en Python:  
```python
for i in range(5):  # Repite 5 veces
    print("Iteración", i)
```

---

### **📍 Iteraciones Anidadas (bucles dentro de bucles)**  
✔️ Se usan para recorrer estructuras más complejas como matrices.  

Ejemplo en Python:  
```python
for i in range(3):
    for j in range(3):
        print(f"Posición ({i}, {j})")
```

---

## **📌 5. Condiciones que Deben Cumplirse en los Bucles**  
✔️ **Condición de entrada:** Define cuándo comienza el bucle.  
✔️ **Condición de salida:** Determina cuándo debe finalizar.  
✔️ **Variable de control:** Debe actualizarse en cada iteración para evitar bucles infinitos.  

Ejemplo de bucle infinito (evitar):  
```python
x = 1
while x > 0:
    print(x)  # Nunca se detiene porque x siempre es mayor que 0
```

---

# **📢 Conclusión**  
Las **estructuras de control** permiten escribir programas dinámicos y adaptables.  
✔️ **Las decisiones** (`if`, `if-elif-else`) permiten ejecutar código condicionalmente.  
✔️ **Los bucles** (`while`, `for`) permiten repetir tareas de manera eficiente.  
✔️ **Las iteraciones anidadas** son útiles para manejar estructuras complejas.  


-------
> **Introducción a la Programación**  
> Python es un lenguaje de programación ideal para principiantes gracias a su sintaxis simple y clara. Con Python, aprenderás conceptos básicos de programación que te ayudarán a resolver problemas y desarrollar aplicaciones en distintas áreas, como ciencia de datos y desarrollo web.