# Jump Runner — Android

Gioco mobile endless runner 2D pronto per essere aperto in Android Studio.

## Funzioni
- Schermata iniziale con artwork/icone del gioco e pulsante **INIZIA**.
- Corsa automatica.
- Un tocco = salto.
- Due tocchi = doppio salto.
- Ostacoli generati all'infinito.
- Monete raccoglibili: ogni moneta vale 100 punti bonus.
- Punteggio progressivo anche durante la corsa.
- Velocità e difficoltà aumentano progressivamente.
- Game Over e pulsante RIGIOCA.
- Icona Android inclusa in più risoluzioni.
- Pubblicità interstitial predisposta con **ID TEST** Google Mobile Ads.

## Pubblicità
Gli ID AdMob presenti nel progetto sono esclusivamente ID TEST. Prima di distribuire l'app, sostituiscili con i tuoi ID AdMob e configura il consenso/privacy richiesto per gli utenti.

## Come ottenere l'APK
1. Apri la cartella `JumpRunner` in Android Studio.
2. Attendi la sincronizzazione Gradle.
3. Seleziona `Build > Generate App Bundle(s) / APK(s) > Generate APK(s)`.
4. Per Google Play usa una build firmata tramite `Generate Signed App Bundle / APK`.

## Struttura
- `app/src/main/assets/index.html` — gameplay.
- `app/src/main/assets/icon.png` — artwork usato nella schermata iniziale.
- `app/src/main/res/mipmap-*` — icone launcher.
- `MainActivity.kt` — WebView + integrazione pubblicità.


## Compilazione direttamente da GitHub

1. Crea un repository GitHub, ad esempio `jump-runner`.
2. Carica tutti i file di questa cartella nella root del repository (la cartella `app` deve stare nella root).
3. Vai in **Actions** e seleziona **Build Jump Runner APK**.
4. Premi **Run workflow**.
5. Quando termina, apri la run completata e scarica l'artifact **JumpRunner-debug-apk**.
6. Dentro troverai `app-debug.apk`, installabile su Android.

Il workflow compila automaticamente il progetto usando JDK 17, Android SDK 35 e Gradle 8.11.1.

### Pubblicità
Il progetto usa attualmente gli ID **TEST** di Google Mobile Ads. Prima di una pubblicazione reale su Google Play sostituiscili con i tuoi ID AdMob.
