# cuestionario-numpy
<h1 align="center">📘 Cuestionario de NumPy – Python Backend</h1>

<p align="center">
Guía de repaso sobre conceptos fundamentales de la librería <strong>NumPy</strong> en Python. Incluye preguntas de opción múltiple, respuestas correctas y explicaciones clave para reforzar el aprendizaje en el desarrollo backend con Python.
</p>

---

<h2 align="center">🧪 Preguntas y Respuestas</h2>

<h3>1️⃣ ¿Qué función se utiliza para crear un array de ceros de tamaño 4x3?</h3>
✅ <code>np.zeros((4, 3))</code>  
🔎 <em>Crea un array de ceros de 4 filas por 3 columnas. Ideal para inicializar estructuras vacías.</em>

---

<h3>2️⃣ ¿Cuál es la diferencia principal entre una lista de Python y un array de NumPy?</h3>
✅ <code>NumPy es más eficiente para cálculos numéricos</code>  
🔎 <em>Los arrays están optimizados a nivel de bajo nivel (C/C++) y permiten operaciones vectorizadas.</em>

---

<h3>3️⃣ ¿Cuál es el resultado de <code>np.ones((2,2)) * 5</code>?</h3>
✅ <code>Matriz de unos multiplicada por 5</code>  
🔎 <em>Resultado: matriz [[5, 5], [5, 5]]. Cada uno se multiplica por 5.</em>

---

<h3>4️⃣ ¿Qué devuelve <code>array.shape</code>?</h3>
✅ <code>Tupla con las dimensiones del array</code>  
🔎 <em>Por ejemplo, un array de 3x2 devolverá (3, 2).</em>

---

<h3>5️⃣ ¿Cuál es el resultado de <code>np.arange(5).reshape(5,1)</code>?</h3>
✅ <code>Un array de 5x1 con los números del 0 al 4</code>  
🔎 <em>Genera una columna con 5 filas: [[0], [1], ..., [4]].</em>

---

<h3>6️⃣ ¿Qué operación suma todos los elementos de un array?</h3>
✅ <code>arr.sum()</code>  
🔎 <em>Suma todos los elementos del array sin importar su forma.</em>

---

<h3>7️⃣ ¿Qué función se utiliza para ordenar un array?</h3>
✅ <code>np.sort()</code>  
🔎 <em>Devuelve una copia ordenada del array (sin modificar el original).</em>

---

<h3>8️⃣ ¿Cuál es el valor de <code>np.mean([1, 2, 3, 4])</code>?</h3>
✅ <code>2.5</code>  
🔎 <em>Media aritmética = (1+2+3+4)/4 = 2.5</em>

---

<h3>9️⃣ ¿Qué representa <code>dtype</code> en un array NumPy?</h3>
✅ <code>Tipo de dato de los elementos</code>  
🔎 <em>Ejemplo: int32, float64, bool, etc.</em>

---

<h3>🔟 ¿Qué función convierte todos los elementos del array a enteros?</h3>
✅ <code>astype(int)</code>  
🔎 <em>Convierte los datos a tipo entero sin modificar el array original.</em>

---

<h3>1️⃣1️⃣ ¿Cómo se cuentan los valores nulos (<code>np.nan</code>) en un array?</h3>
✅ <code>np.isnan(arr).sum()</code>  
🔎 <em>np.isnan devuelve un array booleano. Luego se suman los True (que valen 1).</em>

---

<h3>1️⃣2️⃣ ¿Qué hace <code>np.unique(arr)</code>?</h3>
✅ <code>Devuelve los elementos no repetidos</code>  
🔎 <em>Filtra y devuelve una lista ordenada de elementos únicos.</em>

---

<h3>1️⃣3️⃣ ¿Qué hace <code>np.array([[1, 2], [3, 4]])[1][0]</code>?</h3>
✅ <code>Devuelve 3</code>  
🔎 <em>Accede al elemento en fila 1, columna 0 (índices base cero).</em>

---

<h3>1️⃣4️⃣ ¿Cuál es el resultado de <code>arr[arr > 10]</code> si <code>arr = np.array([5, 10, 15, 20])</code>?</h3>
✅ <code>[15, 20]</code>  
🔎 <em>Filtra los elementos mayores a 10.</em>

---

<h3>1️⃣5️⃣ ¿Qué devuelve <code>np.where(arr % 2 == 0)</code> en un array de enteros?</h3>
✅ <code>Los índices donde los valores son pares</code>  
🔎 <em>Devuelve una tupla con los índices de los elementos que cumplen la condición.</em>

---

<h3>1️⃣6️⃣ ¿Qué hace <code>arr * 2</code> en NumPy si <code>arr = np.array([1, 2, 3])</code>?</h3>
✅ <code>Multiplica cada elemento por 2</code>  
🔎 <em>Resultado: [2, 4, 6].</em>

---

<h3>1️⃣7️⃣ ¿Qué devuelve <code>arr[arr % 2 == 1]</code>?</h3>
✅ <code>Los valores que son impares</code>  
🔎 <em>Filtra solo los números cuyo módulo con 2 sea 1.</em>

---

<h3>1️⃣8️⃣ Si <code>a = np.array([1, 2, 3])</code> y <code>b = np.array([4, 5, 6])</code>, ¿qué devuelve <code>a + b</code>?</h3>
✅ <code>[5, 7, 9]</code>  
🔎 <em>Se realiza una suma elemento a elemento.</em>

---

<h3>1️⃣9️⃣ ¿Cuál es la diferencia entre <code>np.mean(array)</code> y <code>np.nanmean(array)</code>?</h3>
✅ <code>np.mean lanza error si hay np.nan, np.nanmean los ignora al calcular</code>  
🔎 <em><code>nanmean</code> es ideal cuando trabajamos con datos faltantes.</em>

---

<h3>2️⃣0️⃣ ¿Qué hace <code>np.where(np.isnan(array), 0, array)</code>?</h3>
✅ <code>Reemplaza los valores NaN con 0 y deja el resto igual</code>  
🔎 <em>Muy útil para limpiar datos antes de procesarlos.</em>
