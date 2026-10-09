# JARVIS Móvil — PWA 1.0

Esta versión es una aplicación web instalable, no un APK. Incluye comandos básicos de texto, voz sintetizada y reconocimiento de voz si el navegador lo permite. No incorpora aún un modelo de IA.

## Instalar desde Android sin computadora

1. Descarga y descomprime este ZIP en tu celular.
2. Para instalar como aplicación, **debes publicar el contenido de la carpeta en un hosting HTTPS** (por ejemplo, mediante un repositorio GitHub y GitHub Pages). Abrir `index.html` directamente desde Archivos no permite instalar la PWA correctamente.
3. Abre la dirección HTTPS publicada en Chrome para Android.
4. Usa el menú ⋮ → **Añadir a pantalla de inicio** o **Instalar aplicación** (según aparezca).
5. Concede permiso de micrófono cuando se solicite. El reconocimiento de voz depende del navegador y puede requerir conexión a internet.

## Publicación opcional con GitHub Pages

Crea un repositorio público en github.com, sube **los archivos de esta carpeta en la raíz del repositorio** y en Settings → Pages elige Deploy from a branch → main / (root). Espera la publicación y abre la URL HTTPS indicada en Pages. Esto puede hacerse desde el navegador del celular, aunque subir varios archivos puede ser incómodo. No subas contraseñas ni claves privadas.

## Limitaciones

No controla el sistema Android ni escucha en segundo plano. Los comandos funcionan sin IA externa. Algunas funciones de voz requieren internet y/o soporte del navegador. No hay servidor remoto ni cuenta requerida.
