# REFERENCIA JAVASCRIPT
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=flat&logo=javascript&logoColor=%23F7DF1E) ![Markdown](https://img.shields.io/badge/markdown-%23000000.svg?style=flat&logo=markdown&logoColor=white)

## VARIABLES
En JavaScript, las Variables se Utilizan para almacenar diferentes Tipos de Datos. Aquí están los principales tipos de variables:

1. **Number**: Representa tanto números enteros como decimales.
   - Ejemplo:
     ```javascript
     let num = 42;
     let decimal = 3.14; //revizar este.
     ```

2. **String**: Cadenas de texto, encerradas entre comillas simples (`' '`), dobles (`" "`), o con backticks (`` ` ``).
   - Ejemplo:
     ```javascript
     let texto = 'Hola';
     let saludo = `Hola, ${nombre}';
     ```

3. **Boolean**: Almacenan valores lógicos: `true` o `false`.
   - Ejemplo:
     ```javascript
     let esVerdad = true;
     ```

4. **Undefined**: El valor por defecto de una variable declarada pero no inicializada.
   - Ejemplo:
     ```javascript
     let variableSinValor; // undefined
     ```

5. **Null**: Representa la ausencia intencional de un valor.
   - Ejemplo:
     ```javascript
     let valorNulo = null;
     ```

6. **Object**: Tipo complejo que puede almacenar colecciones de datos y más tipos de valores.
   - Ejemplo: 
     ```javascript
     let persona = {
       nombre: "Juan",
       edad: 30
     };
     ```

7. **Array**: Tipo especial de objeto usado para almacenar listas de valores.
   - Ejemplo:
     ```javascript
     let lista = [1, 2, 3, "cuatro"];
     ```

8. **Symbol**: Representa un valor único y es utilizado para crear identificadores únicos para objetos.
   - Ejemplo:
     ```javascript
     let simbolo = Symbol('descripcion');
     ```

9. **BigInt**: Permite trabajar con números enteros más grandes que el límite de `Number`.
   - Ejemplo:
     ```javascript
     let numeroGrande = BigInt(9007199254740991);
     ```

Estos son los tipos básicos, aunque se pueden combinar y extender para casos más avanzados.

## OPERADORES
En JavaScript, los Operadores se Utilizan para realizar Operaciones en Variables y Valores. Aquí están los principales tipos de operadores que te permiten manipular valores y realizar cálculos:

1. **Operadores Aritméticos**: Realizan operaciones matemáticas.
   - `+` (suma)
   - `-` (resta)
   - `*` (multiplicación)
   - `/` (división)
   - `%` (módulo)
   - `++` (incremento)
   - `--` (decremento)

2. **Operadores de Asignación**: Asignan valores a las variables.
   - `=` (asignación simple)
   - `+=` (asignación y suma)
   - `-=` (asignación y resta)
   - `*=` (asignación y multiplicación)
   - `/=` (asignación y división)
   - `%=` (asignación y módulo)

3. **Operadores de Comparación**: Comparan dos valores.
   - `==` (igual a)
   - `===` (estrictamente igual a)
   - `!=` (no igual a)
   - `!==` (estrictamente no igual a)
   - `>` (mayor que)
   - `<` (menor que)
   - `>=` (mayor o igual que)
   - `<=` (menor o igual que)

4. **Operadores Lógicos**: Operan con valores booleanos.
   - `&&` (AND lógico)
   - `||` (OR lógico)
   - `!` (NOT lógico)

5. **Operadores Bit a Bit**: Trabajan a nivel de bits.
   - `&` (AND bit a bit)
   - `|` (OR bit a bit)
   - `^` (XOR bit a bit)
   - `~` (NOT bit a bit)
   - `<<` (desplazamiento a la izquierda)
   - `>>` (desplazamiento a la derecha)

6. **Operadores de Tipo**: Determinan el tipo de un valor.
   - `typeof` (tipo de)
   - `instanceof` (instancia de)

7. **Operador Ternario**: Es una forma abreviada de una declaración `if-else`.
   - `condición ? expresión1 : expresión2`

8. **Operadores de Cadena**: Operan sobre cadenas de texto.
   - `+` (concatenación)
   - `+=` (asignación y concatenación)

**NOTA OPERADORES**: `++` y `--`

La diferencia entre `variable++` y `++variable` radica en **CUANDO** se incrementa el valor de la `variable`:

1. **`variable++` (Post-incremento)**: Primero se utiliza el valor actual de `variable`, y luego se incrementa. Es decir, se usa el valor de `variable` tal como está en la expresión y después se suma 1 a `variable`.

   ```javascript
   let a = 5;
   let b = a++;  // b = 5, pero a = 6
   ```

   - Primero `b` toma el valor actual de `a` (5), y después `a` se incrementa a 6.

2. **`++variable` (Pre-incremento)**: Primero se incrementa `variable`, y luego se utiliza el nuevo valor. Es decir, `variable` aumenta en 1 antes de usarse en la expresión.

   ```javascript
   let a = 5;
   let b = ++a;  // a = 6, b = 6
   ```

   - Aquí, `a` se incrementa antes de asignar su valor a `b`.

**Resumen:**
- `variable++`: Incrementa **después** de utilizar el valor.
- `++variable`: Incrementa **antes** de utilizar el valor.
  

## CONDICIONALES
En JavaScript, los Condicionales se Utilizan para que el Código Tome Decisiones en función de condiciones específicas. Los principales tipos de condicionales son:

1. **`if`**:
   Se utiliza para ejecutar un bloque de código si una condición es verdadera.
   ```javascript
   if (condición) {
     // código a ejecutar si la condición es verdadera
   }
   ```

2. **`if...else`**:
   Se utiliza para ejecutar un bloque de código si la condición es verdadera, y otro bloque si es falsa.
   ```javascript
   if (condición) {
     // código si la condición es verdadera
   } else {
     // código si la condición es falsa
   }
   ```

3. **`else if`**:
   Permite evaluar múltiples condiciones. Si una condición es verdadera, su bloque de código se ejecuta y el resto se ignora.
   ```javascript
   if (condición1) {
     // código si condición1 es verdadera
   } else if (condición2) {
     // código si condición2 es verdadera
   } else {
     // código si ninguna de las condiciones es verdadera
   }
   ```

4. **`switch`**:
   Evalúa una expresión y ejecuta el bloque de código correspondiente al valor de la expresión.
   ```javascript
   switch (expresión) {
     case valor1:
       // código si la expresión es igual a valor1
       break;
     case valor2:
       // código si la expresión es igual a valor2
       break;
     default:
       // código si la expresión no coincide con ningún caso
   }
   ```

5. **Operador Ternario (`? :`)**:
   Es una forma corta de un `if...else`. Se usa para asignaciones rápidas en función de una condición.
   ```javascript
   condición ? expresiónSiVerdadero : expresiónSiFalso;
   ```

Estos son los principales tipos de condicionales que permiten controlar el flujo de un programa en JavaScript.

## FUNCIONES
En JavaScript, las funciones son Bloques de Código Reutilizables que permiten realizar una tarea específica. Se utilizan para organizar el código, evitar la repetición y facilitar su mantenimiento. existen varias formas de definir funciones, cada una con su propia sintaxis. A continuación se detallan los tipos más comunes:

1. **Declaración de función (Function Declaration)**:
   Es la forma más tradicional de definir una función. Se puede llamar antes de que esté definida en el código debido al "hoisting".
   ```javascript  
   function sumar(a, b) {
     return a + b;
   };
   ```
  
2. **Expresión de función (Function Expression)**:
   Se define como una expresión dentro de una variable. No se puede invocar antes de que se defina.
   ```javascript
   const sumar = function(a, b) {
     return a + b;
   };
   ```

3. **Funciones flecha (Arrow Functions)**:
   Introducidas en ES6, son más concisas y no vinculan su propio valor de `this`.
   ```javascript
   const sumar = (a, b) => a + b;
   ```

4. **Funciones anónimas**:
   Son funciones sin nombre, que suelen usarse como argumentos de otras funciones.
   ```javascript
   setTimeout(function() {
     console.log("Hola después de 2 segundos");
   }, 2000);
   ```

5. **Funciones IIFE (Immediately Invoked Function Expression)**:
   Son funciones que se ejecutan inmediatamente después de ser definidas.
   ```javascript
   (function() {
     console.log("Esto se ejecuta inmediatamente");
   })();
   ```

6. **Métodos dentro de objetos**:
   Las funciones pueden ser propiedades de un objeto.
   ```javascript
   const objeto = {
     saludar: function() {
       console.log("Hola");
     }
   };
   objeto.saludar();
   ```

7. **Funciones generadoras (Generator Functions)**:
   Permiten pausar y reanudar la ejecución de la función mediante `yield`.
   ```javascript
   function* generador() {
     yield 1;
     yield 2;
     yield 3;
   }
   ```

Cada tipo tiene sus ventajas según el caso de uso. Pero las 3 Primeras son las más utilizadas en la mayoría de los escenarios.

## BUCLES
En JavaScript, los Bucles se Utilzan para repetir un bloque de código varias veces hasta que se cumpla una Condición Específica. A continuación, te muestro los tipos de bucles más comunes:

1. El Bucle `for` se utiliza cuando conoces el número de iteraciones por adelantado. Su estructura básica es:

```javascript
for (inicialización; condición; incremento) {
  // Código a ejecutar en cada iteración
}
```

**Ejemplo:**
```javascript
for (let i = 0; i < 5; i++) {
  console.log(i);  // Imprime 0, 1, 2, 3, 4
}
```

2. El Bucle `while` se utiliza cuando no sabes cuántas veces necesitas iterar, pero quieres repetir el bloque mientras se cumpla una condición.

```javascript
while (condición) {
  // Código a ejecutar mientras la condición sea verdadera
}
```

**Ejemplo:**
```javascript
let i = 0;
while (i < 5) {
  console.log(i);
  i++;
}
```

3. El bucle `do...while` es similar al `while`, pero garantiza que el bloque de código se ejecute al menos una vez antes de verificar la condición.

```javascript
do {
  // Código a ejecutar
} while (condición);
```

**Ejemplo:**
```javascript
let i = 0;
do {
  console.log(i);
  i++;
} while (i < 5);
```

4. El Bucle `for...in` Se utiliza para iterar sobre las propiedades enumerables de un objeto.

```javascript
for (let propiedad in objeto) {
  // Código a ejecutar en cada iteración
}
```

**Ejemplo:**
```javascript
const objeto = { nombre: "Juan", edad: 30,  sexo: "masculino"};
for (let clave in objeto) {
  console.log(clave + ": " + objeto[clave]);
}
```

5. El Bucle `for...of` Se utiliza para iterar sobre valores de objetos iterables como arrays, mapas, conjuntos, etc.

```javascript
for (let valor of iterable) {
  // Código a ejecutar en cada iteración
}
```

**Ejemplo:**
```javascript
const numeros = [10, 20, 30];
for (let numero of numeros) {
  console.log(valor);
}
```

Cada bucle tiene su uso particular dependiendo de lo que quieras hacer, como recorrer listas, objetos o realizar acciones repetitivas mientras una condición se mantenga verdadera.
