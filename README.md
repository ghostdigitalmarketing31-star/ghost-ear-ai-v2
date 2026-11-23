# GHOST EAR AI V1

Prototype web/PWA gratuit de comparaison acoustique.

## Ce que fait cette V1
- Enregistre 6 secondes via le microphone du navigateur.
- Calcule RMS, pic, taux de passages par zéro et centre spectral estimé.
- Permet d'enregistrer une référence sonore par machine.
- Compare un nouvel enregistrement à cette référence et signale des écarts.
- Stocke les références dans le navigateur du téléphone.

## Limites importantes
Ce prototype ne diagnostique pas une panne et n'a pas été validé industriellement. Les résultats sont sensibles au téléphone, à la distance, au bruit ambiant, au niveau de charge et aux conditions d'enregistrement. Un résultat « aucun écart » ne prouve pas qu'une machine est saine. Toute alerte doit être vérifiée par un technicien.

## Lancer sur Android gratuitement
Le microphone exige une origine sécurisée HTTPS (ou localhost). Ouvrir le fichier index.html directement depuis le gestionnaire de fichiers ne suffit généralement pas.

### Déploiement gratuit avec GitHub Pages
1. Créer un compte sur github.com ou se connecter.
2. Créer un nouveau dépôt public nommé `ghost-ear-ai`.
3. Téléverser les trois fichiers : `index.html`, `manifest.webmanifest`, `sw.js`.
4. Dans le dépôt, ouvrir Settings > Pages.
5. Dans « Build and deployment », choisir « Deploy from a branch », branche `main`, dossier `/ (root)`, puis Save.
6. Attendre la publication et ouvrir l'adresse HTTPS fournie par GitHub Pages dans Chrome Android.
7. Autoriser le microphone. Dans le menu Chrome, choisir « Ajouter à l'écran d'accueil » ou « Installer l'application » si l'option apparaît.

## Premier test recommandé
- Choisir une machine accessible et stable.
- Enregistrer à distance fixe, dans un environnement calme.
- Créer une référence lorsque la machine fonctionne normalement.
- Faire un deuxième enregistrement dans les mêmes conditions.
- Tester ensuite des sons différents uniquement dans un cadre sûr et autorisé.

Les données sont locales au navigateur. Effacer les données du site ou changer de téléphone peut faire perdre les références.
