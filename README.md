# KM Find Madrid

Página web de **KM Find Madrid**: compras personales en España con envío a Colombia.
Bolsos, perfumes, zapatillas, makeup, skincare y Pandora, 100% originales.

Instagram: [@kmfind_madrid](https://www.instagram.com/kmfind_madrid/)

## Contenido

- `index.html`: la página completa (diseño, catálogo y botones de WhatsApp).
- `img/`: logo, fotos de portada y fotos de los productos.

## Publicar gratis con GitHub Pages

1. Sube estos archivos a un repositorio de GitHub.
2. En el repositorio entra a **Settings → Pages**.
3. En **Source** elige **Deploy from a branch**, rama `main` y carpeta `/ (root)`. Guarda.
4. En uno o dos minutos la página queda en `https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/`.

## Cambios frecuentes

**Número de WhatsApp.** En `index.html` busca esta línea y pon el número con indicativo, sin espacios ni `+`:

```js
const WHATSAPP = "";   // ejemplo: "34600123456"
```

Si queda vacío, los botones llevan a Instagram.

**Productos y precios.** En `index.html` busca `const P = [`. Cada producto es una línea:

```js
{c:"bolsos", b:"Michael Kors", n:"Bandolera Gigi", img:"bolso1", p:580000},
```

- `c`: categoría (`bolsos`, `zapatillas`, `perfumes` o `pandora`)
- `b`: marca
- `n`: nombre del modelo
- `img`: nombre de la foto dentro de `img/` (sin `.jpg`)
- `p`: precio en pesos colombianos

Etiqueta opcional: agrega `tag:"Más pedido"`, `tag:"Nuevo"` o `tag:"Últimas unidades"` al producto.

Para perfumes con varios tamaños se usa `s` en lugar de `p`:

```js
s:[["50 ml",320000],["90 ml",375000]]
```

© 2026 KM Find Madrid. Todos los derechos reservados.
