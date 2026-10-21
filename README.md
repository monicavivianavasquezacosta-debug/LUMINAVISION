# Lumina Visión · Landing de venta

Página de una sola pantalla para vender gafas. Los pedidos y consultas llegan por WhatsApp.
Es HTML, CSS y JavaScript puros: no necesita instalar nada.

## Qué editar (todo en `index.html`)

Busca el bloque `EDITA AQUÍ` casi al final del archivo:

```js
const CONFIG = {
  whatsapp: "",            // Ejemplo Colombia: "573001234567" (indicativo + número, sin + ni espacios)
  products: [
    {shape:"round", name:"Redonda", desc:"...", price:"", img:""},
    ...
  ]
};
```

- `whatsapp`: tu número. Sin esto los botones abren WhatsApp sin destinatario.
- `price`: precio en texto, por ejemplo `"$ 289.000"`. Vacío muestra "Consulta el precio".
- `img`: ruta de una foto, por ejemplo `"assets/redonda.jpg"`. Vacío muestra el dibujo de la montura.
- Para un quinto modelo, copia una línea de producto. Formas disponibles: `round`, `square`, `aviator`, `cat`.

Los textos de preguntas frecuentes y de "Cómo comprar" están en el HTML; reemplázalos con tus políticas reales de pago, envíos y cambios.

## Publicar gratis con GitHub Pages

1. Crea un repositorio nuevo en github.com (por ejemplo `lumina-vision`), público.
2. Sube todo el contenido de esta carpeta: `index.html`, la carpeta `assets` y `.nojekyll`.
   (En la página del repositorio: **Add file → Upload files**, arrastra los archivos y pulsa **Commit changes**.)
3. Ve a **Settings → Pages**. En **Source** elige **Deploy from a branch**, rama `main`, carpeta `/ (root)` y pulsa **Save**.
4. En 1 o 2 minutos tendrás tu página en `https://TU-USUARIO.github.io/lumina-vision/`.

### Dominio propio (opcional)

En **Settings → Pages → Custom domain** escribe tu dominio (por ejemplo `luminavision.co`) y configura en tu proveedor un registro `CNAME` hacia `TU-USUARIO.github.io`. Activa **Enforce HTTPS**.

## Estructura

```
index.html
assets/
  hero.mp4        video de inicio (655 KB)
  poster.jpg      imagen mientras carga el video
  favicon.svg     icono de la pestaña
  og-logo.svg     logo sobre fondo oscuro
.nojekyll
```

## Marca

Paleta: tinta `#0E1A33`, marino `#1F3A6B`, cobalto `#2F5DA8`, latón `#B58A3C` y `#D9B26A`, niebla `#E8ECF2`.
Tipografía: Jost (titulares) y Source Serif 4 (texto), desde Google Fonts.
