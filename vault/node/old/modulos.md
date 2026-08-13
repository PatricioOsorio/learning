---
icon: "🚀"
---

# Exportaciones (`module.exports`)

---

```javascript
const sumar = (n1, n2) => n1 + n2;
const restar = (n1, n2) => n1 - n2;
const multiplicar = (n1, n2) => n1 * n2;

module.exports = { sumar, restar, multiplicar };
```

# Importaciones (`require`)

---

- Importa contenido de otros archivos

- Es necesario el punto (`.`)

```javascript
const variable = require("./Direccion");
```

# Ejemplo

---

## frutas.js

```javascript
const frutas = ["platano", "manzada", "pera"];
const dinero = 1000;

//Exportar
module.exports = { frutas, dinero };
```

## app.js

```javascript
// Importar
// Mediante destructuracion de objeto
const { frutas, dinero } = require("./frutas");
```
