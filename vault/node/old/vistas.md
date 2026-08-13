---
icon: "💻"
---

# ¿Que es?

---

- Existe una manera dinámica de crear nuestro sitios

- Usando motores de plantillas

Entre los más populares:

- ejs

- hbs

- hjs

- jade

- pug

- twig|vash

# Motores de plantilla

---

Para que Express pueda representar archivos de plantilla, deben establecerse los
siguientes valores de aplicación:

views, el directorio donde se encuentran los archivos de plantilla. Ejemplo:
app.set('views', './views')

view engine, el motor de plantilla que se utiliza. Ejemplo: app.set('view engine', 'pug')

**EJEMPLOS COMPATIBLES CON EXPRESS**

[Template Engines (expressjs.com)](https://expressjs.com/en/resources/template-engines.html)

# Ejemplos

---

## Pug

```bash
if tareas.length
	each tarea in tareas
		li.tarea (data-tarea = `${tarea. id}` )
			p= tarea.tarea
```

## Handlebars

```html
<div class="caja">
  <p class="etiqueta">Empresa:</p>
  <p class="nombre">{{vacante.empresa}}</p>
</div>
<div class="caja">
  <p class="etiqueta">Ubicacion:</p>
  <p class="nombre">{{vacante.ubicacion}}</p>
</div>
```

## EJS

```html
<div class="informacion-usuario">
  <div class="imagen">
    <% if(usuario.imagen) { %>
    <img src="/uploads/perfiles/<%= usuario.imagen %>" alt="" />
    <% } %>
  </div>
  <div class="texto"><%- usuario.descripcion %></div>
</div>
```

# EJS y Express

- Embedded JavaScript Templateting

- No perdemos nuestro html clásico y agregamos lógica con EJS.

## Instalacion

```bash
npm install ejs
```
