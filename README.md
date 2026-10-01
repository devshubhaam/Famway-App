# FamWay app (Capacitor)

Ye app tumhari Koyeb site ko Android/iOS app me wrap karta hai. Dashboard wahi dikhega jo site par hai.
Site me change karoge to app update karne ki zaroorat nahi, wo seedha live dikhega.

## APK banane ka sabse aasaan tarika (laptop/Android Studio ke bina)
1. Is folder (`famway-app`) ko ek naye GitHub repo me daalo.
2. GitHub -> Actions -> "Build Android APK" -> Run workflow.
3. Khatam hone par "famway-debug-apk" artifact download karo, zip kholo, `app-debug.apk` phone me install karo.

## Laptop se banana
    npm install
    npx cap add android
    npx cap sync android
    npx cap open android      # Android Studio khulega, Build -> Build APK

## Domain badalne par
`capacitor.config.json` me `server.url` aur `allowNavigation` ka address badlo, phir `npx cap sync`.
