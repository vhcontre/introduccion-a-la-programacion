# **UNIDAD III: Subprogramas y Funciones**  

## **🧩 Módulos y Programación Modular**  

### 📌 **¿Qué es un módulo?**  
Un **módulo** es un bloque de código independiente que puede reutilizarse en diferentes partes de un programa. Permite dividir un programa en secciones más manejables y organizadas.  

### 🏗️ **Ventajas de la Programación Modular**  
✔️ **Reutilización**: Se pueden usar las mismas funciones en varios programas.  
✔️ **Legibilidad**: Facilita la comprensión del código al dividirlo en partes más pequeñas.  
✔️ **Mantenimiento**: Permite modificar una parte del código sin afectar el resto del programa.  
✔️ **Trabajo en equipo**: Diferentes programadores pueden trabajar en distintos módulos al mismo tiempo.  

### 🔧 **Desarrollo de Programas de Forma Modular**  
Se logra separando el código en **módulos** y utilizando **procedimientos y funciones**.  

---

## **🔹 Procedimientos y Funciones**  

### 📜 **¿Qué es un procedimiento?**  
Un **procedimiento** es un bloque de código que realiza una tarea específica pero **no devuelve un valor**.  

Ejemplo en Python:  
```python
def saludar():
    print("¡Hola, bienvenido!")
```

### 📌 **¿Qué es una función?**  
Una **función** es un bloque de código que realiza una tarea y **devuelve un valor**.  

Ejemplo en Python:  
```python
def sumar(a, b):
    return a + b
```

### 🔄 **Diferencias y Semejanzas entre Procedimientos y Funciones**  

| Característica       | Procedimiento 🏗️ | Función 🎯 |
|---------------------|----------------|-------------|
| Devuelve un valor  | ❌ No | ✅ Sí |
| Uso principal | Ejecutar una tarea | Calcular y devolver un resultado |
| Ejemplo de uso | Mostrar un mensaje en pantalla | Calcular la suma de dos números |

---

## **📌 Tipos de Funciones**  

### 🔹 **Funciones Estándar**  
Son funciones que vienen incorporadas en los lenguajes de programación.  

Ejemplos en Python:  
✔️ `print()` – Muestra texto en pantalla.  
✔️ `len()` – Retorna la longitud de una lista o cadena.  
✔️ `round()` – Redondea un número.  

### 🔹 **Funciones Definidas por el Usuario**  
Son funciones creadas por el programador para realizar tareas específicas.  

Ejemplo:  
```python
def cuadrado(numero):
    return numero * numero
```

---

## **📌 Variables y Parámetros en Funciones**  

### 🌍 **Variables Globales y Locales**  
📌 **Variable Global**: Se define fuera de una función y puede ser usada en todo el programa.  
📌 **Variable Local**: Se define dentro de una función y solo puede ser utilizada en ella.  

Ejemplo en Python:  
```python
mensaje = "Hola"  # Variable global

def mostrar_mensaje():
    mensaje_local = "Bienvenido"  # Variable local
    print(mensaje_local)

print(mensaje)  # Se puede acceder
mostrar_mensaje()
# print(mensaje_local)  # Esto generará un error, ya que es una variable local
```

### 📌 **Parámetros en Funciones**  

#### 📍 **Parámetros Formales**  
Son los nombres de las variables que se usan en la declaración de una función.  

Ejemplo:  
```python
def saludo(nombre):  # 'nombre' es un parámetro formal
    print(f"Hola, {nombre}")
```

#### 📍 **Paso de Parámetros**  

✔️ **Por Valor**: Se envía una copia del valor original y no se modifica la variable externa.  
✔️ **Por Variable (Referencia)**: Se pasa la dirección de la variable, por lo que los cambios afectan a la variable original.  

Ejemplo de paso por valor:  
```python
def doblar(numero):
    numero = numero * 2
    return numero

valor = 5
print(doblar(valor))  # Devuelve 10
print(valor)  # Sigue siendo 5 (no se modificó)
```

Ejemplo de paso por referencia (listas en Python):  
```python
def modificar_lista(lista):
    lista.append(100)

numeros = [1, 2, 3]
modificar_lista(numeros)
print(numeros)  # La lista ahora incluye 100
```

---

## **📢 Conclusión**  
Las funciones y procedimientos permiten dividir un programa en partes reutilizables y organizadas. La programación modular facilita el mantenimiento del código y mejora su estructura. Comprender el uso de variables globales y locales, así como el paso de parámetros, es esencial para escribir programas eficientes y flexibles.

-------
> **Introducción a la Programación**  
> Python es un lenguaje de programación ideal para principiantes gracias a su sintaxis simple y clara. Con Python, aprenderás conceptos básicos de programación que te ayudarán a resolver problemas y desarrollar aplicaciones en distintas áreas, como ciencia de datos y desarrollo web.