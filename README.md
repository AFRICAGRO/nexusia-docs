# nexusia-docs
Documentation for NexusIA API (NexusIA Docs)

## Versions installables

Ce dépôt est maintenant prêt pour deux modes d’installation sur mobile :

1. PWA installable (Android, Chrome)
2. Wrapper Android via Capacitor

## PWA installable

Ouvrez le site dans Chrome sur Android puis :
- Menu ⋮
- Installer l’application
- Confirmer l’installation

Le site est également compatible avec l’ajout à l’écran d’accueil sur mobile.

## Wrapper Android (Capacitor)

1. Installer les dépendances :
   npm install

2. Ajouter la plateforme Android :
   npx cap add android

3. Synchroniser le web avec Android :
   npm run cap:sync

4. Ouvrir Android Studio :
   npm run cap:open

5. Générer une APK ou un bundle Android depuis Android Studio.

## Déploiement local

Pour tester localement :

python3 -m http.server 8080

Puis ouvrir : http://localhost:8080

## Fichiers clés

- index.html : interface de documentation
- manifest.webmanifest : configuration PWA
- sw.js : cache et service worker
- capacitor.config.ts : configuration de wrapper Android
- openapi.yaml : spécification OpenAPI de démonstration

## Notes

- Le fichier OpenAPI est un exemple de départ.
- Remplacez l’URL API dans `openapi.yaml` ou le backend réel selon votre environnement.
