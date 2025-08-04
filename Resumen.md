
### **Tabla Resumen de Variables en JavaScript**

| **Tipo**       | **Declaración**       | **Alcance**       | **Reasignable** | **Re-declarable** | **Hoisting** | **Valor por defecto** |
|----------------|-----------------------|------------------|-----------------|-------------------|--------------|-----------------------|
| `var`          | `var x;`              | Función          | Sí              | Sí                | Sí           | `undefined`           |
| `let`          | `let x;`              | Bloque (`{}`)    | Sí              | No                | No*          | `undefined`           |
| `const`        | `const x = valor;`    | Bloque (`{}`)    | No**            | No                | No*          | Requiere inicialización |
| **Sin clave*** | `x = 10;` (no recomendado) | Global (no recomendado) | Sí | Sí | Sí | - |

---

### **Explicación Breve:**
1. **`var`**:
   - Alcance de función (o global si se declara fuera).
   - Permite re-declaración y re-asignación.
   - Sufre hoisting (se declara, pero no se inicializa).

2. **`let`**:
   - Alcance de bloque (dentro de `{}`).
   - No permite re-declaración en el mismo bloque, pero sí re-asignación.
   - No sufre hoisting (error si se usa antes de declarar).

3. **`const`**:
   - Alcance de bloque.
   - No permite re-asignación ni re-declaración.
   - Debe inicializarse al declararla.
   - Para objetos/arrays, sus propiedades/elementos internos sí pueden modificarse.

4. **Sin clave** (no recomendado):
   - Variable global (se añade al objeto `window` en navegadores).
   - Mala práctica por contaminación del scope global.

---

### **Ejemplos:**
```javascript
var a = 1;      // Puede ser re-declarada y re-asignada
let b = 2;      // Solo re-asignable, no re-declarable
const c = 3;    // No se puede re-asignar ni re-declarar

// Ejemplo con const y objetos:
const obj = { nombre: "Juan" };
obj.nombre = "Pedro";  // ✅ Válido (mutación interna)
// obj = { nombre: "Ana" };  // ❌ Error (reasignación)
```

> **Notas**:
> - **Hoisting**: `var` se declara al inicio del scope (pero no se inicializa), `let`/`const` no.
> - **Bloque**: Cualquier estructura con `{}` (if, for, funciones, etc.).
> - **`const`**: Para tipos primitivos (number, string, etc.) es inmutable, pero para objetos/arrays permite mutaciones internas.


