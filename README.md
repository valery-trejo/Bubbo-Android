# bubbo — App Android

La página `index.html` está en `app/src/main/assets/index.html`, idéntica a la original.
La app es un contenedor WebView nativo (Java) con adaptaciones solo del lado Android.

## Generar el APK (elige una opción)

### Opción A — Android Studio
1. Abre la carpeta `bubbo-android` con Android Studio (Hedgehog o más nuevo).
2. Espera a que termine "Gradle Sync".
3. Menú **Build > Build Bundle(s) / APK(s) > Build APK(s)**.
4. El APK queda en `app/build/outputs/apk/release/app-release.apk`.

### Opción B — Línea de comandos
Requiere JDK 17, Android SDK y Gradle 8.7:

    gradle assembleRelease

### Opción C — Sin instalar nada (GitHub Actions)
1. Sube esta carpeta a un repositorio nuevo de GitHub.
2. Pestaña **Actions > Build APK > Run workflow**.
3. Descarga `bubbo-apk` desde "Artifacts" (contiene `bubbo.apk`).

## Instalar
Copia el APK al teléfono y ábrelo (activa "Instalar apps desconocidas" si lo pide).
