---
icon: "⏲️"
---

# Crear promesa

---

```javascript
const promesa = new Promise((res, rej) => {
  res("Exito en la promesa");
  rej("Fracaso en la promesa");
});

promesa.then((res) => {
  console.log(res);
});
promesa.catch((err) => {
  console.log(err);
});
```
