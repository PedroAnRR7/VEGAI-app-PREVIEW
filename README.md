<p align="center">
  <img src="assets/portada.png" alt="VEGAI — tu asistente de IA" width="100%">
</p>

<h1 align="center">
  <img src="assets/icono.png" width="44" align="center" alt=""> VEGAI
</h1>

<p align="center">
  <b>Tu asistente de IA personal: los principales modelos de inteligencia artificial, en un solo lugar.</b><br>
  Android · Windows — de <b>ROMER Interactive</b>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/versi%C3%B3n-1.0.0-5b3fd9" alt="Versión 1.0.0">
  <img src="https://img.shields.io/badge/Android-7.0%2B-3ddc84?logo=android&logoColor=white" alt="Android 7.0+">
  <img src="https://img.shields.io/badge/Windows-10%2F11-0078d4?logo=windows&logoColor=white" alt="Windows 10/11">
  <img src="https://img.shields.io/badge/c%C3%B3digo-privado-555" alt="Código privado">
</p>

---

## Qué es

VEGAI es un asistente de IA para el día a día: preguntas rápidas, traducir, resumir documentos o revisar un correo. Se abre directamente en el chat, sin cuentas ni registros, y por debajo combina varios modelos de IA gratuitos: si uno falla o está saturado, cambia a otro automáticamente sin que el usuario lo note.

| Inicio | Documentos | Modo oscuro | Privacidad |
|---|---|---|---|
| <img src="assets/01-inicio.png" width="200"> | <img src="assets/02-documentos.png" width="200"> | <img src="assets/03-oscuro.png" width="200"> | <img src="assets/04-privacidad.png" width="200"> |

## Funciones

- **Chat al estilo de los grandes asistentes**, con sugerencias de consulta rápida y respuestas en tiempo real.
- **Lee documentos e imágenes**: PDF, Word, Excel, PowerPoint, texto y código, con el texto extraído **en el propio dispositivo**.
- **Conversaciones con contexto** y un resumen automático de cada una en el historial.
- **Privacidad de verdad**: todo se guarda **solo en el dispositivo, cifrado con AES-256** (clave en Android Keystore o Windows DPAPI). Chat temporal, borrado automático de adjuntos a los 7 días y bloqueo con huella.
- **Varios modelos, una sola app**: Qwen, GPT-OSS, Llama y Mistral, con cambio automático entre proveedores si uno falla.
- **Diseño cuidado**: glassmorphism, claro y oscuro, transiciones fluidas y adaptado a móvil, tableta y escritorio.
- **Gratuita**: 10 conversaciones nuevas por semana con mensajes ilimitados en cada una; si necesitas más, basta con ver un vídeo corto.

## Descargas

| Plataforma | Dónde |
|---|---|
| **Android** | Google Play *(próximamente)* · APK en [Releases](../../releases) |
| **Windows 10/11** | Instalador de un clic en [Releases](../../releases) |

## Cómo está hecha

| Parte | Tecnología |
|---|---|
| Interfaz | React 19, TypeScript, Vite 8, Tailwind CSS 4 |
| Android | Capacitor 8 (API 36) con plugins nativos en Java: streaming HTTP, Android Keystore + biometría y color de las barras del sistema. Compactado con R8: APK de 4,5 MB |
| Windows | Electron 38 con un servidor de enrutado de modelos integrado e instalador NSIS de un clic |
| Seguridad | Cifrado AES-256-GCM (WebCrypto) sobre IndexedDB, Android Keystore y Windows DPAPI |
| Documentos | pdf.js y fflate (Office/ODF), procesados en el dispositivo |
| IA | Enrutador propio con puntuación por calidad y velocidad, reintentos y pausas por modelo cuando un proveedor limita |
| Monetización | Google AdMob (banner, nativo y bonificado) con consentimiento RGPD (UMP) |

## Créditos

- **Desarrollo y publicación:** ROMER Interactive.
- **Código:** Pedro Antonio Ruiz Romero.
- Construida sobre **[FreeLLMAPI](https://github.com/tashfeenahmed/freellmapi)** de **Tashfeen Ahmed** (licencia MIT).
- Los modelos de IA pertenecen a sus autores y se usan bajo sus licencias (Qwen, GPT-OSS y Mistral: Apache 2.0; Llama 3.3: Llama 3.3 Community License — *Built with Llama*).

---

<p align="center">
  <a href="https://sites.google.com/view/vegai-privacidad">Política de privacidad</a> · Contacto: <a href="mailto:romerinteractive@gmail.com">romerinteractive@gmail.com</a>
</p>

<p align="center"><sub>© 2026 ROMER Interactive. El código fuente de VEGAI es privado; este repositorio solo presenta la aplicación y distribuye sus instaladores.</sub></p>
