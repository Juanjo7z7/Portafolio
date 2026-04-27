# Portafolio · Juan José Arbeláez

Sitio web personal — Full Stack Developer.

🌐 **Demo:** _agrega aquí el link cuando hagas deploy_

---

## Stack

- HTML5 semántico
- CSS3 (custom properties, grid, flexbox)
- JavaScript vanilla (sin frameworks)
- Google Fonts (Instrument Serif · Newsreader · DM Mono)

Sin build step, sin dependencias, sin `node_modules`. Todo carga con una petición HTML + CSS + JS.

---

## Estructura

```
.
├── index.html          ← Página principal
├── assets/
│   ├── styles.css      ← Estilos
│   └── script.js       ← Smooth scroll + active nav
├── README.md
└── .gitignore
```

---

## Subirlo a GitHub Pages

### 1. Crear el repo

1. Andá a [github.com/new](https://github.com/new)
2. Nombre: `portafolio` (o `tu-usuario.github.io` para usar la URL `https://tu-usuario.github.io`)
3. Marcalo como **Public**
4. NO marques "Initialize with README"
5. Clic en **Create repository**

### 2. Subir los archivos

En la terminal, dentro de la carpeta del proyecto:

```bash
git init
git add .
git commit -m "Primera versión del portafolio"
git branch -M main
git remote add origin https://github.com/TU-USUARIO/NOMBRE-DEL-REPO.git
git push -u origin main
```

> Reemplazá `TU-USUARIO` y `NOMBRE-DEL-REPO`.

### 3. Activar GitHub Pages

1. En el repo → **Settings** (pestaña arriba)
2. Menú izquierdo → **Pages**
3. Source: **Deploy from a branch**
4. Branch: `main` · folder: `/ (root)` · **Save**
5. Esperá 1-2 minutos. La URL queda:

   ```
   https://TU-USUARIO.github.io/NOMBRE-DEL-REPO/
   ```

---

## Probarlo localmente

```bash
# con Python
python3 -m http.server 8000

# con Node
npx serve

# abrí http://localhost:8000
```

Abrir `index.html` con doble clic también funciona.

---

## Editar el contenido

Todo el copy está en `index.html`. Para cambiar colores, editá las variables al inicio de `assets/styles.css`:

```css
:root {
  --paper:        #F2EEE5;   /* fondo */
  --ink:          #14110F;   /* texto */
  --ink-soft:     #423D36;
  --ink-muted:    #7A736A;
  ...
}
```

Después de cualquier cambio:

```bash
git add .
git commit -m "Describe el cambio"
git push
```

GitHub Pages se actualiza solo en ~1 minuto.

---

## Dominio personalizado (opcional)

Si tenés un dominio propio:

1. En tu DNS, agregá un CNAME apuntando a `TU-USUARIO.github.io`
2. En GitHub → Settings → Pages → escribí tu dominio en *Custom domain*
3. Marcá *Enforce HTTPS*

---

Juan José Arbeláez Castro · 2026
