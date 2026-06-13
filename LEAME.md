# Planeador Didáctico · Cultura Digital I — Cómo publicarlo (versión corregida)

Ya **no se necesita ninguna carpeta**. Solo dos archivos, juntos, en la raíz del repositorio:

```
index.html        ← la aplicación (debe llamarse exactamente así)
activities.json   ← el banco de actividades (mismo nombre, junto a index.html)
```

## Cómo dejar tu repositorio GENERADOR-SEC03 correcto

1. Entra a tu repositorio en GitHub.
2. **Borra** los archivos que sobran o confunden:
   - `índice.html` (con acento, no sirve como inicio)
   - `actividades.json` si lo subiste con ese nombre (lo reemplazaremos por `activities.json`)
3. **Sube** estos dos archivos nuevos a la raíz:
   - `index.html`  (este archivo es la app; antes se llamaba `planeador_cultura_digital_I.html`)
   - `activities.json`
   > Si ya tienes `planeador_cultura_digital_I.html`, puedes simplemente **renombrarlo** a `index.html` (botón editar ✏️ → cambiar el nombre) y borrar `índice.html`.
4. El archivo principal **tiene que llamarse `index.html`** (minúsculas, en inglés). Así GitHub Pages muestra la app al entrar.

## Activar el sitio (GitHub Pages)

1. En el repositorio: **Settings → Pages**.
2. *Build and deployment* → **Deploy from a branch** → rama `main` → carpeta `/ (root)` → **Save**.
3. Espera 1–2 minutos. Tu app quedará en:
   ```
   https://jonatanpowerj-crypto.github.io/GENERADOR-SEC03/
   ```

## El banco se carga solo

Como `activities.json` está junto a `index.html`, al abrir el sitio la app **carga el banco automáticamente** (verás en la pestaña Banco el aviso "✓ Banco cargado automáticamente desde el sitio"). No tienes que pegar ninguna URL.

Si quieres más actividades: edita `activities.json` en GitHub, agrega objetos con un `id` único, guarda, y recarga la página.

## Comprobaciones rápidas

- Al entrar a `https://jonatanpowerj-crypto.github.io/GENERADOR-SEC03/` debe verse la app (no una lista de archivos). Si ves la lista, el archivo no se llama `index.html`.
- En la pestaña **Banco** debe aparecer el aviso verde de carga automática. Si no, revisa que `activities.json` esté en la raíz y bien escrito.

---
Nota: tus planes y tu avance se guardan en el navegador del dispositivo; no se envían a ningún servidor.
