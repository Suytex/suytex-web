# Changelog — suytex-web

Registro de cambios del sitio. Más reciente arriba.

## 2026-07-02

### WhatsApp: ocultar número, unificar estilo verde
- Nav, CTA final y botón flotante ahora usan el mismo estilo verde WhatsApp (`.btn-wa` / `.btn-wa-sm`)
- Se quitó el número visible del CTA final (antes mostraba `809-408-9999`) y del `aria-label`
- Se agregó label dinámico "Empezar ahora →" en el CTA final, coherente con el mensaje precargado de esa sección
- Número ofuscado en base64 dentro del script (`atob(...)`) — ya no aparece como texto plano en el HTML. Los 3 links (`waNav`, `waCtaFinal`, `waFab`) se construyen en runtime desde ese único punto
- Nota: es ofuscación, no seguridad real — el número sigue siendo visible en DevTools/Network al hacer clic
