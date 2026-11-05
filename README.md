# KouizzeuhApp

Application Android en Kotlin de quiz : création ou rejoindre une partie, lobby, déroulement du jeu et classement.

## Ouvrir et compiler

Prévoir Android Studio, un JDK compatible avec le plugin Android Gradle 8.x du dépôt et le SDK Android 33. La configuration `app/build.gradle `déclare `compileSdk 33` et `minSdk 27`.

1. Cloner le dépôt et ouvrir sa racine dans Android Studio.
2. Installer le SDK demandé et synchroniser Gradle.
3. Depuis la racine, compiler un APK de développement :

```bash
bash gradlew :app:assembleDebug
```

Sous Windows : `gradlew.bat :app:assembleDebug`. Le wrapper Gradle est fourni. L'APK est produit dans `app/build/outputs/apk/debug/` si la compilation réussit.

Les sources utilisent Firebase. Configurer un projet Firebase adapté à votre installation et son fichier local `app/google-services.json`, ainsi que les services et règles requis. Ne pas réutiliser des identifiants de production pour les essais.

## Vérification

Les versions et commandes ci-dessus ont été contrôlées par lecture de la configuration. Compilation, tests Android et fonctionnement sur appareil non exécutés.
