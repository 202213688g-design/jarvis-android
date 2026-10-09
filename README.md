# JARVIS 2.0 para Android (PWA)

## Actualizar desde el celular
1. Abre https://github.com/202213688g-design/jarvis-android en Chrome e inicia sesión.
2. Pulsa **Add file → Upload files** (en móvil puede estar dentro del menú de tres puntos).
3. **Descomprime este ZIP** y sube los archivos que contiene a la **raíz** del repositorio (no subas el ZIP ni la carpeta contenedora). Los archivos `index.html`, `manifest.webmanifest`, `sw.js`, `icon.svg`, `icon-192.png`, `icon-512.png` y `README.md` reemplazan los anteriores; `app.js` es nuevo.
4. Confirma con **Commit changes**. GitHub Pages publicará la nueva versión automáticamente. Espera unos minutos y abre https://202213688g-design.github.io/jarvis-android/ . Si ves la versión anterior, cierra la aplicación y recarga la página (o borra caché del sitio).
5. En Chrome: menú ⋮ → **Instalar aplicación** o **Añadir a pantalla de inicio**.

## Funciones
- Chat con comandos locales y enlaces a búsquedas.
- Reconocimiento de voz si Chrome lo permite; requiere permisos y puede necesitar internet.
- Respuestas por síntesis de voz del navegador (la voz disponible depende del celular).
- Personalidad configurable y memoria editable guardada localmente en `localStorage`.
- Exportación de datos y eliminación del historial/memoria.
- Integración opcional con servidor de IA externo vía HTTPS.

## IA real: contrato del servidor
El sitio de GitHub Pages es estático y **no contiene claves API**. Para IA real configura un servidor propio y seguro que acepte `POST` JSON con `{message, memory, personality, history}` y responda `{ "reply": "texto" }`. El servidor debe permitir CORS exclusivamente desde tu dominio GitHub Pages y autenticar solicitudes; CORS por sí solo NO es autenticación. El servidor debe guardar la clave del proveedor de IA en sus variables secretas y aplicar límites de uso. No introduzcas claves privadas en el campo de URL ni en GitHub.

Si no tienes servidor, **JARVIS sigue funcionando en modo local** y no finge ser una IA avanzada. Los mensajes y memoria solo salen del dispositivo si configuras un servidor externo.

## Limitaciones
- No es una APK nativa. El navegador no puede controlar libremente otras apps ni escuchar permanentemente en segundo plano.
- La memoria es local a este navegador/dispositivo y se pierde si borras los datos del sitio.
- No proporciona diagnósticos médicos, hackeo, pilotaje autónomo ni control físico de hardware.
