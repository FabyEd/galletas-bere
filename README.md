# Bere & Miga — sitio web

Sitio de una sola página hecho con HTML, CSS y JavaScript simple (sin frameworks ni build tools). No necesita instalación de nada para funcionar.

## Estructura de archivos

```
├── index.html          ← todo el contenido y estructura de la página
├── css/
│   └── style.css       ← todos los estilos (colores, tipografías, layout)
├── js/
│   └── main.js         ← solo controla el menú móvil (hamburguesa)
├── images/              ← fotos de los cakes + favicon
└── README.md            ← este archivo
```

## Cómo ver el sitio en tu computadora (antes de publicarlo)

No necesitas instalar nada especial. Simplemente:

1. Descomprime la carpeta si viene en `.zip`.
2. Haz doble clic en `index.html`. Se abrirá en tu navegador.

Eso es todo — así puedes revisar cambios antes de subirlos a internet.

## Qué es lo primero que debes cambiar

Este es un **borrador**. Antes de publicarlo de verdad, busca estos puntos marcados con comentarios `REEMPLAZAR` dentro de `index.html`:

1. **Datos de contacto** (sección `Contacto`, cerca del final del archivo):
   - Número de WhatsApp real (`https://wa.me/593999999999` → reemplaza los números por el número real, sin espacios ni signos, con código de país).
   - Usuario real de Instagram.
   - Correo real.
2. **Fotos**: ya están subidas `vainilla.jpg`, `genoise.png` y las tres fotos del huerto (`huerto-limon.jpg`, `huerto-maracuya.jpg`, `huerto-pina.jpg`). La galería de "Nuestro huerto" por ahora solo muestra esas tres frutas porque no hay foto de mango — si consigues una, guárdala como `images/huerto-mango.jpg` y avisa para agregarla a la galería.
   - También puedes reemplazar `chocolate.jpg`, `naranja.jpg`, `banana.jpg`, `maracuya.jpg` y `zanahoria.jpg` por versiones de mejor resolución si las tienes; basta con guardar el archivo nuevo con el mismo nombre.

El sitio es informativo: no muestra la receta completa (ingredientes ni paso a paso) de ningún sabor, solo una descripción breve.

## Cómo editar el contenido

Todo el texto visible está directamente en `index.html`, organizado en secciones con comentarios como:

```html
<!-- =========================================================
     SABORES / CATÁLOGO
     ========================================================= -->
```

Para cambiar una descripción, un título o un texto, simplemente edita el texto entre las etiquetas correspondientes (por ejemplo `<h3>Chocolate</h3>`) con cualquier editor de texto (Bloc de notas, TextEdit, o mejor aún, [Visual Studio Code](https://code.visualstudio.com/), que es gratis).

Para cambiar colores o tipografías, todo está centralizado al inicio de `css/style.css`, en la sección `:root { ... }` — cambia el valor hexadecimal de cualquier color y se actualiza en todo el sitio.

## Cómo publicarlo gratis en GitHub Pages

GitHub Pages te da hosting gratuito para sitios estáticos como este, sin necesidad de dominio propio (tu sitio quedará en una dirección como `https://tu-usuario.github.io/galletas-bere/`).

### Paso 1: Crear una cuenta de GitHub (si no tienes una)
Ve a [github.com](https://github.com) y crea una cuenta gratuita.

### Paso 2: Crear un repositorio nuevo
1. Haz clic en el botón **"New"** (o el **+** arriba a la derecha → "New repository").
2. Ponle un nombre, por ejemplo `galletas-bere`.
3. Déjalo como **Public** (público) — es requisito para GitHub Pages gratis.
4. No marques ninguna opción adicional (README, .gitignore, etc.). Haz clic en **"Create repository"**.

### Paso 3: Subir los archivos del sitio
En la página del repositorio recién creado:
1. Haz clic en **"uploading an existing file"** (o el botón "Add file" → "Upload files").
2. Arrastra **todos** los archivos y carpetas de este proyecto (`index.html`, la carpeta `css`, la carpeta `js`, la carpeta `images`) — mantén la misma estructura de carpetas.
3. Baja y haz clic en **"Commit changes"**.

### Paso 4: Activar GitHub Pages
1. En el repositorio, ve a **Settings** (Configuración) → **Pages** (en el menú de la izquierda).
2. En "Branch", selecciona `main` y la carpeta `/ (root)`.
3. Haz clic en **Save**.
4. Espera 1-2 minutos. GitHub te mostrará la URL pública del sitio, algo como:
   `https://tu-usuario.github.io/galletas-bere/`

¡Y listo! Esa URL ya la puedes compartir con tus clientas.

### Para actualizar el sitio después
Cada vez que quieras cambiar algo, edita el archivo localmente y vuelve a subirlo (Add file → Upload files, reemplazando el archivo existente) o, si prefieres una forma más profesional, aprende a usar Git desde la terminal o [GitHub Desktop](https://desktop.github.com/) (con interfaz visual, más fácil para no programadores).

## Nota sobre las fuentes (tipografías)

El sitio usa Google Fonts (Caveat, Fraunces y Karla), que se cargan automáticamente desde internet cuando alguien visita la página — no necesitas instalar nada, solo funciona mientras la persona tenga conexión a internet (algo normal hoy en día).
