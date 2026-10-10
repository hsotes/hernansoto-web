# Ejercicios de estructuras

Biblioteca de ejercicios de cálculo estructural hechos a partir de fotos de estructuras reales.
Es una carpeta del repositorio `hsotes/hernansoto-web` y se publica con GitHub Pages en **https://hernansoto.com/estructuras/**.

## Estructura del repositorio

```
estructuras/
├── index.html                    ← índice con una tarjeta por ejercicio
└── columna-semaforica/
    └── index.html                ← cada ejercicio es una página autónoma (foto incluida)
```

Las páginas llevan `<meta name="robots" content="noindex, nofollow">`: son públicas para quien tenga el enlace, pero los buscadores no las listan.

## Cómo agregar un ejercicio nuevo

1. Crear una carpeta con un nombre corto, en minúsculas y con guiones (ejemplo: `puente-peatonal`).
2. Guardar adentro la página del ejercicio como `index.html`.
   - Si el archivo viene de un artifact de Claude (sin `<!doctype html>`, `<head>` ni `<body>`),
     envolverlo igual que `columna-semaforica/index.html`: agregar `<!doctype html>`, `<html lang="es">`,
     `<head>` con `charset`, `viewport` y `<meta name="robots" content="noindex, nofollow">`, y `<body>`.
   - Agregar el enlace "← Ejercicios de estructuras" (`href="../"`) arriba de todo.
3. En `index.html` (el índice), copiar una tarjeta `<a class="card">` y ponerla **primera** en la lista,
   con número correlativo, fecha, lugar, título, una línea de descripción y los temas.
4. Subir los cambios:

   ```
   git add .
   git commit -m "Agrega ejercicio: <nombre>"
   git push
   ```

   En uno o dos minutos queda publicado en `https://hernansoto.com/estructuras/<carpeta>/`.

## Ejercicios

| # | Ejercicio | Temas |
|---|-----------|-------|
| 01 | [Columna semafórica con pescante](https://hernansoto.com/estructuras/columna-semaforica/) | Viento CIRSOC 102, flexión + torsión CIRSOC 301, placa base, pernos, dado H-21 |
