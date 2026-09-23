# StudentWay — page de téléchargement

Site statique (une page) déployé sur Vercel. L'APK Android n'est **pas** dans ce dépôt :
il est attaché aux **Releases** GitHub de ce dépôt, sous le nom exact `StudentWay.apk`.

Lien de téléchargement utilisé par la page (toujours la dernière version) :
https://github.com/lemeti/studentway-download/releases/latest/download/StudentWay.apk

## Publier une nouvelle version de l'APK
1. `flutter build apk --release` (avec les mêmes `--dart-define` que d'habitude).
2. GitHub → ce dépôt → **Releases** → **Draft a new release**.
3. Tag : `v0.2.0` (par exemple) → glisser l'APK **renommé en `StudentWay.apk`** → **Publish release**.
4. Dans `index.html`, bloc « RÉGLAGES » en bas : mettre à jour `VERSION` et `TAILLE`, puis commit.
   Vercel redéploie tout seul.
