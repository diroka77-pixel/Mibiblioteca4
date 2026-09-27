# Mi Biblioteca v0.4

Aplicación Android en Kotlin + Jetpack Compose para catalogar una carpeta de archivos EPUB accesible mediante el selector de documentos de Android (incluido Google Drive cuando su proveedor aparece en el selector).

## Funciones
- Selección persistente de carpeta con Storage Access Framework.
- Escaneo recursivo de archivos `.epub`.
- Lectura de metadatos OPF: título, autor, fecha, editorial, género, descripción, ISBN y saga cuando estén presentes.
- Extracción de portada EPUB cuando está declarada en el OPF.
- Búsqueda y filtros.
- Ficha detallada y apertura con una app compatible con EPUB.

## Compilar
1. Abrir esta carpeta con Android Studio.
2. Usar JDK 17 y dejar que Android Studio sincronice Gradle.
3. Instalar Android SDK 35 si Android Studio lo solicita.
4. Build > Build APK(s).

> Nota: esta entrega no incluye un APK precompilado porque el entorno donde se generó el proyecto no dispone de Android SDK/Gradle para verificar una compilación real.

## APK con GitHub Actions
Al subir estos archivos a la rama `main`, la pestaña Actions ejecuta «Compilar APK». Cuando termine, abre la ejecución y descarga el artefacto «MiBiblioteca-v0.4-debug». Contiene `app-debug.apk` (versión de prueba).
