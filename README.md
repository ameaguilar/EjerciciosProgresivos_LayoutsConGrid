# EjerciciosProgresivos_LayoutsConGrid
En los siguientes ejercicios  se emplea el uso de Grids y  Box Model en CSS y HTML

# Ejercicios de CSS Grid

Colección de ejercicios prácticos para aprender y practicar **CSS Grid**, desde la creación de una cuadrícula básica hasta la construcción de layouts responsive.

---

## Ejercicio 1 — Mi primera Grid

### Objetivo

Crear una cuadrícula de **6 elementos**, distribuidos en 3 columnas y 2 filas.

```text
┌──────┬──────┬──────┐
│  1   │  2   │  3   │
├──────┼──────┼──────┤
│  4   │  5   │  6   │
└──────┴──────┴──────┘
```

### Requisitos

Utilizar las siguientes propiedades:

```css
display: grid;
grid-template-columns;
gap;
```

### Restricción

> No utilizar **Flexbox**.

---

## Ejercicio 2 — Cambiando la estructura

Partiendo de los mismos elementos, deberán modificar la estructura de la cuadrícula utilizando únicamente:

```css
grid-template-columns;
```

### A — 2 columnas

```text
1  2
3  4
5  6
```

### B — 3 columnas

```text
1  2  3
4  5  6
```

### C — 4 columnas

```text
1  2  3  4
5  6  7  8
```

### Restricción

**Solo pueden modificar:**

```css
grid-template-columns;
```

---

## Ejercicio 3 — Dashboard

Tenemos los siguientes elementos:

* Ventas
* Usuarios
* Pedidos
* Productos
* Soporte
* Reportes

### Objetivo

Construir el siguiente dashboard:

```text
┌────────────┬────────────┬────────────┐
│   Ventas   │  Usuarios  │  Pedidos   │
├────────────┼────────────┼────────────┤
│ Productos  │  Soporte   │  Reportes  │
└────────────┴────────────┴────────────┘
```

### Requisitos

El ejercicio debe utilizar:

* `display: grid`
* 3 columnas
* `gap`
* Box Model
* `:hover`

---

## Ejercicio 4 — Tarjeta destacada

Ahora deberán crear una tarjeta destacada utilizando CSS Grid.

### Resultado esperado

```text
┌──────────────────────┬──────────┐
│                      │          │
│      DESTACADA       │  CARD 2  │
│                      │          │
├──────────┬───────────┴──────────┤
│  CARD 3  │       CARD 4         │
└──────────┴───────────────────────┘
```

### Requisitos

La tarjeta destacada deberá ocupar **2 columnas** utilizando:

```css
grid-column: span 2;
```

---

## Ejercicio 5 — Página web con Grid Areas

### Objetivo

Construir la siguiente estructura de página:

```text
┌─────────────────────────────────┐
│             HEADER              │
├────────────┬────────────────────┤
│            │                    │
│    MENU    │      CONTENT       │
│            │                    │
│            │                    │
├────────────┴────────────────────┤
│             FOOTER              │
└─────────────────────────────────┘
```

### Requisitos

Deben utilizar las siguientes propiedades:

```css
grid-template-columns;
grid-template-areas;
grid-area;
gap;
```

La estructura deberá estar organizada mediante **Grid Areas**.

---

## Ejercicio 6 — Responsive

### Objetivo

Partiendo del ejercicio anterior, deberán adaptar la página para que funcione correctamente en pantallas pequeñas.

### Vista de escritorio

Mantener la estructura del ejercicio anterior:

```text
┌─────────────────────────────────┐
│             HEADER              │
├────────────┬────────────────────┤
│    MENU    │      CONTENT       │
├────────────┴────────────────────┤
│             FOOTER              │
└─────────────────────────────────┘
```

### Vista móvil

Cuando la pantalla sea pequeña, la estructura deberá cambiar a:

```text
┌──────────────────┐
│      HEADER      │
├──────────────────┤
│       MENU       │
├──────────────────┤
│     CONTENT      │
├──────────────────┤
│      FOOTER      │
└──────────────────┘
```

### Requisitos

En este ejercicio pueden utilizar:

```css
@media
```

y modificar:

```css
grid-template-areas;
```

### Ejemplo

```css
@media (max-width: 600px) {

    .pagina {
        grid-template-columns: 1fr;

        grid-template-areas:
            "header"
            "menu"
            "contenido"
            "footer";
    }
}
```

---

## Objetivo final

Al completar estos ejercicios, deberán ser capaces de:

* Crear layouts utilizando **CSS Grid**.
* Definir columnas y filas.
* Utilizar `gap` para controlar el espacio entre elementos.
* Hacer que un elemento ocupe varias columnas.
* Organizar layouts mediante `grid-template-areas`.
* Utilizar `grid-area`.
* Crear diseños **responsive** con `@media`.
* Combinar Grid con conceptos del **Box Model** y estados como `:hover`.

> **Regla general:** intenta resolver cada ejercicio utilizando únicamente las propiedades indicadas en sus requisitos.
