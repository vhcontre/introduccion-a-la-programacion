# **📌 Funciones en Programación**  

## **🖥️ 1. Funciones**  
✔️ Bloques de código reutilizables que realizan una tarea específica.  
✔️ Se pueden ejecutar múltiples veces sin reescribir el código.  
✔️ Permiten estructurar mejor los programas.  

Ejemplo en Python:  
```python
def saludar():
    print("¡Hola, bienvenido!")

saludar()  # Llamado a la función
```

---

## **📂 2. Módulos**  
✔️ Son archivos que contienen funciones y código reutilizable.  
✔️ Facilitan la organización del código en programas grandes.  
✔️ Se pueden importar con `import`.  

Ejemplo en Python:  
```python
import math  # Módulo de funciones matemáticas
print(math.sqrt(16))  # Uso de una función del módulo
```

---

## **💡 3. Ventajas de la Programación Modular**  
✔️ **Reutilización de código**: No es necesario escribir el mismo código varias veces.  
✔️ **Mantenimiento más sencillo**: Se pueden modificar funciones sin afectar el resto del código.  
✔️ **Legibilidad**: El código es más claro y estructurado.  
✔️ **Colaboración**: Diferentes personas pueden trabajar en módulos separados.  

---

## **📌 4. Desarrollo de Programas de Forma Modular**  
📌 Se basa en la descomposición del problema en módulos o funciones independientes.  
📌 Cada función realiza una tarea específica y el programa principal coordina su ejecución.  

Ejemplo:  
```python
def sumar(a, b):
    return a + b

def restar(a, b):
    return a - b

# Programa principal
num1 = 10
num2 = 5
print("Suma:", sumar(num1, num2))
print("Resta:", restar(num1, num2))
```

---

## **🔹 5. Procedimientos y Funciones**  

### **📍 Procedimientos**  
✔️ Subrutinas que ejecutan instrucciones pero **no devuelven valores**.  
✔️ En Python, se implementan con `def` sin `return`.  

Ejemplo en Python:  
```python
def mostrar_mensaje():
    print("Esto es un procedimiento")

mostrar_mensaje()  # No devuelve ningún valor
```

---

### **📍 Funciones**  
✔️ Similar a los procedimientos, pero **devuelven un valor** con `return`.  

Ejemplo en Python:  
```python
def cuadrado(num):
    return num * num

resultado = cuadrado(4)  # Guarda el valor retornado
print(resultado)  # Imprime 16
```

---

## **📌 6. Funciones Estándar**  
📌 Python tiene muchas funciones predefinidas que facilitan la programación.  

Ejemplos:  
✔️ `print()` → Muestra información en pantalla.  
✔️ `len()` → Devuelve la longitud de una lista o cadena.  
✔️ `sum()` → Suma todos los elementos de una lista.  

```python
lista = [1, 2, 3, 4]
print(len(lista))  # Imprime 4
print(sum(lista))  # Imprime 10
```

---

## **📌 7. Funciones Definidas por el Usuario**  
📌 Son funciones creadas por el programador según las necesidades del programa.  

Ejemplo:  
```python
def multiplicar(a, b):
    return a * b

print(multiplicar(3, 4))  # Devuelve 12
```

---

## **📌 8. Diferencias y Semejanzas entre Procedimientos y Funciones**  

| Característica | Procedimientos | Funciones |
|--------------|--------------|------------|
| Devuelven un valor | ❌ No | ✅ Sí |
| Se llaman igual | ✅ Sí | ✅ Sí |
| Se utilizan para modularizar código | ✅ Sí | ✅ Sí |
| Uso de `return` | ❌ No | ✅ Sí |

---

## **📌 9. Variables en Funciones**  

### **📍 Variables Globales**  
✔️ Se definen fuera de cualquier función.  
✔️ Pueden ser accedidas y modificadas por cualquier parte del programa.  
✔️ Se deben evitar en exceso porque pueden generar errores difíciles de depurar.  

Ejemplo:  
```python
contador = 0  # Variable global

def incrementar():
    global contador
    contador += 1
    print(contador)

incrementar()  # Modifica la variable global
```

---

### **📍 Variables Locales**  
✔️ Se definen dentro de una función y solo existen dentro de ella.  
✔️ No afectan ni pueden ser accedidas desde fuera de la función.  

Ejemplo:  
```python
def calcular():
    resultado = 10  # Variable local
    print(resultado)

calcular()
# print(resultado)  # Esto generaría un error porque la variable no existe fuera de la función
```

---

## **📌 10. Parámetros en Funciones**  

📌 **Son valores que se envían a una función cuando se la llama.**  
📌 Existen dos tipos principales: **por valor** y **por referencia**.  

### **📍 Parámetros por Valor**  
✔️ Se pasa una copia del valor a la función, sin afectar la variable original.  

Ejemplo:  
```python
def duplicar(numero):
    numero = numero * 2  # Modifica la copia, no la original
    return numero

n = 5
print(duplicar(n))  # Devuelve 10
print(n)  # Sigue siendo 5
```

---

### **📍 Parámetros por Referencia (por variable)**  
✔️ Se pasa la referencia a la variable original, por lo que **puede ser modificada dentro de la función**.  
✔️ En Python, **las listas y diccionarios** se pasan por referencia.  

Ejemplo:  
```python
def modificar_lista(lista):
    lista.append(100)  # Modifica la lista original

numeros = [1, 2, 3]
modificar_lista(numeros)
print(numeros)  # Ahora es [1, 2, 3, 100]
```

---

# **📢 Conclusión**  
✔️ **Las funciones** permiten estructurar y organizar mejor los programas.  
✔️ **Los módulos** ayudan a reutilizar código y hacer que los programas sean más mantenibles.  
✔️ **Diferenciar funciones y procedimientos** ayuda a elegir la mejor estrategia según la necesidad.  
✔️ **El uso correcto de variables locales y globales** es clave para evitar errores.  
✔️ **Los parámetros por valor y por referencia** permiten modificar o mantener los datos según sea necesario.  


-------
> **Introducción a la Programación**  
> Python es un lenguaje de programación ideal para principiantes gracias a su sintaxis simple y clara. Con Python, aprenderás conceptos básicos de programación que te ayudarán a resolver problemas y desarrollar aplicaciones en distintas áreas, como ciencia de datos y desarrollo web.