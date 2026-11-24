# Audio Extractor (Windows · Zero-Python)

Utilidad nativa ultrarrápida para Windows (**1 archivo `.bat`, sin Python ni dependencias**) diseñada para extraer la pista de audio de videos pesados (grabaciones de OBS Studio, clases, reuniones, etc.) con solo **arrastrar y soltar**.

Ideal como paso previo para reducir archivos de **1.5 GB a ~50 MB (-96%)** en pocos segundos antes de subirlos a herramientas de transcripción web como **[Transcriptor Suite](https://github.com/Klopezxd/transcriptor-suite)**.

---

### ⬇️ Descarga Directa

👉 **[Descargar última versión (`extraer_audio.bat`)](https://github.com/Klopezxd/audio-extractor/releases/latest/download/extraer_audio.bat)**

---

### Características

* **Extracción instantánea sin pérdida (`Stream Copy`):** Usa `-vn -c:a copy` con FFmpeg para separar la pista de audio original sin recodificar (toma ~2 segundos en videos compatibles).
* **Respaldo automático inteligente:** Si el contenedor o códec del video no permite copia directa, recodifica automáticamente a **AAC Mono 64 kbps (`.m4a`)** optimizado para voz.
* **Cero Python / Cero instalación:** Funciona de forma nativa en Windows 10/11.
* **Detección y autoinstalación de FFmpeg en 1 clic:**
  * Busca `ffmpeg.exe` automáticamente en carpeta portable (`bin\`), `PATH`, `WinGet`, `Conda`, `Scoop` y `Chocolatey`.
  * Si no tienes FFmpeg instalado, ofrece descargarlo automáticamente en modo portable o instalarlo vía `WinGet`.
* **Procesamiento por lotes:** Puedes arrastrar uno o múltiples videos a la vez sobre `extraer_audio.bat`.

---

### Cómo usar

1. Descarga **[`extraer_audio.bat`](https://github.com/Klopezxd/audio-extractor/releases/latest/download/extraer_audio.bat)**.
2. Arrastra uno o varios videos directamente encima del archivo `extraer_audio.bat` (o ábrelo con doble clic y pega la ruta del video).
3. Si es tu primera vez y no tienes FFmpeg, escribe `S` cuando te pregunte si deseas instalarlo automáticamente.
4. En segundos se creará un archivo `<nombre_video>_audio.m4a` junto a tu video original.

---

### Licencia

[MIT License](LICENSE) — © 2026 [Klever López](https://github.com/Klopezxd)
