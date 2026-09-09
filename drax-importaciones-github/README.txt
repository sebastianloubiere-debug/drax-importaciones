DRAX IMPORTACIONES - PWA PARA GITHUB PAGES

Estos archivos están listos para subir al repositorio drax-importaciones.
La app instalable abre dentro de la PWA la Web App de Google Apps Script que ya funciona.
Por eso sigue usando la misma planilla de Google Sheets y no hay que cambiar el backend.

ARCHIVOS A SUBIR A GITHUB:
- index.html
- manifest.json
- service-worker.js
- icon-192.png
- icon-512.png

PASOS:
1. Entrar al repositorio drax-importaciones en GitHub.
2. Add file > Upload files.
3. Arrastrar LOS CINCO ARCHIVOS anteriores (no subir la carpeta cerrada ni el ZIP).
4. Commit changes.
5. Ir a Settings > Pages.
6. En Build and deployment / Source elegir Deploy from a branch.
7. Branch: main. Folder: /(root). Guardar.
8. Esperar 1-3 minutos.
9. GitHub mostrará una dirección similar a:
   https://TU-USUARIO.github.io/drax-importaciones/
10. Abrir ESA dirección en Chrome de Android.
11. Menú de Chrome > Instalar aplicación / Agregar a pantalla principal.

IMPORTANTE:
- El Apps Script actual debe seguir publicado como Web App.
- Su doGet debe usar setXFrameOptionsMode(HtmlService.XFrameOptionsMode.ALLOWALL), como ya está configurado.
- Si modificás el código interno de la app en Apps Script, seguís publicando una nueva versión allí. No hace falta volver a instalar la PWA.
