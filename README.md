# hernansoto.com

Sitio de Hernán Soto Escalante, publicado con GitHub Pages desde este repositorio (`hsotes/hernansoto-web`) en el dominio propio **hernansoto.com** (archivo `CNAME`).

## Contenido

```
/
├── index.html        ← portada (por ahora, "sitio en construcción")
├── CNAME             ← dominio propio: hernansoto.com
├── .nojekyll         ← GitHub Pages sirve los archivos tal cual
└── estructuras/      ← biblioteca de ejercicios de estructuras
```

- La portada se va a reemplazar por el sitio de servicios.
- `estructuras/` se publica en https://hernansoto.com/estructuras/. No está enlazada desde la portada y sus páginas llevan `noindex`: las ve quien tenga el enlace, pero los buscadores no las listan. Ver `estructuras/README.md`.

## Publicar un cambio

```
git add .
git commit -m "Descripción del cambio"
git push
```

En uno o dos minutos queda publicado.

## Si el sitio se muda a otro servicio

Hay que llevar también la carpeta `estructuras/`, para que sus direcciones sigan funcionando.
