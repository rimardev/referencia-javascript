# REFERENCIA JAVASCRIPT
![JavaScript](https://img.shields.io/badge/javascript-%23323330.svg?style=flat&logo=javascript&logoColor=%23F7DF1E) ![Markdown](https://img.shields.io/badge/markdown-%23000000.svg?style=flat&logo=markdown&logoColor=white)

## VARIABLES
En JavaScript, las variables pueden almacenar diferentes tipos de datos. Aquí están los principales tipos de variables:

1. **Number**: Representa tanto números enteros como decimales.
   - Ejemplo: `let num = 42;` o `let decimal = 3.14;`

2. **String**: Cadenas de texto, encerradas entre comillas simples (`' '`), dobles (`" "`), o con backticks (`` ` ``).
   - Ejemplo: `let texto = 'Hola';` o ``let saludo = `Hola, ${nombre}`;``

3. **Boolean**: Almacenan valores lógicos: `true` o `false`.
   - Ejemplo: `let esVerdad = true;`

4. **Undefined**: El valor por defecto de una variable declarada pero no inicializada.
   - Ejemplo: `let variableSinValor; // undefined`

5. **Null**: Representa la ausencia intencional de un valor.
   - Ejemplo: `let valorNulo = null;`

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
   - Ejemplo: `let simbolo = Symbol('descripcion');`

9. **BigInt**: Permite trabajar con números enteros más grandes que el límite de `Number`.
   - Ejemplo: `let numeroGrande = BigInt(9007199254740991);`

Estos son los tipos básicos, aunque se pueden combinar y extender para casos más avanzados.
