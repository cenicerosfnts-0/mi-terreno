# 🏡 Mi Terreno

App para iPhone que lleva el control de los pagos del terreno en **El Porvenir de Degollado**.
Los datos viven en tu hoja de Google Sheets; esta página solo es la app.

## 1. Prepara tu hoja (en la compu)

1. Abre tu hoja → **Extensiones → Apps Script**, pega el `MiTerreno.gs` nuevo y guarda.
2. Ejecuta `instalar` una vez (tus pagos se conservan).
3. En la hoja: menú **🏡 Mi Terreno → 🔐 Configurar PIN de la app** y elige un PIN de 4 a 8 dígitos.
4. En Apps Script: **Implementar → Gestionar implementaciones → ✏️ Editar**
   - Ejecutar como: **Yo**
   - Quién tiene acceso: **Cualquier usuario**
   - Versión: **Nueva versión** → Implementar
5. Copia el link que termina en **/exec**.

> Sin el PIN, el link no entrega ni modifica nada. Tras 8 intentos fallidos se bloquea 15 minutos.

## 2. Publica la app en GitHub Pages

1. En github.com crea un repositorio nuevo llamado `mi-terreno` (público).
2. **Add file → Upload files** y sube todos los archivos de esta carpeta.
3. **Settings → Pages** → Source: *Deploy from a branch* → Branch: `main` / `(root)` → Save.
4. En 1–2 minutos queda en `https://TU-USUARIO.github.io/mi-terreno/`.

El repositorio no guarda ningún dato tuyo: el link y el PIN se guardan solo en tu iPhone.

## 3. Instálala en tu iPhone

1. Abre `https://TU-USUARIO.github.io/mi-terreno/` en **Safari**.
2. Pega tu link `/exec` y tu PIN → **Conectar**.
3. **Compartir → Agregar a pantalla de inicio**. Aparece con el ícono de Mi Terreno.

## Cómo se usa

- **＋** registra un pago (con foto del comprobante). Los billetes vuelan a la bolsa 💰 y la bolsa llena el aro de la casita 🏡.
- **Pagos**: toca un pago para editarlo, deslízalo a la izquierda para borrarlo.
- **Plan**: tus 20 fechas, del enganche a la liquidación.
- Toca la **casita** para cambiar entre modo Automático, Claro u Oscuro.

## Actualizar la app

Sube el `index.html` nuevo al repositorio. Si cambias otros archivos, sube también `sw.js` con un número de versión nuevo (`mi-terreno-v2`, etc.).
