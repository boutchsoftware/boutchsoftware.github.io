# boutchsoftware.github.io

Site racine de l'organisation **BoutchSoftware** sur GitHub Pages.

Rôles :

- **`/.well-known/assetlinks.json`** — déclaration des App Links Android. C'est ce fichier
  qui permet aux étiquettes NFC de « Touché, c'est fait » d'ouvrir directement l'application,
  sans dialogue « Ouvrir avec… ». Chaque nouvelle app BoutchSoftware utilisant des App Links
  s'ajoute comme entrée supplémentaire dans ce tableau JSON.
- **`/touchefait/t/`** — page de secours affichée quand une étiquette est touchée par un
  téléphone **sans** l'application. L'identifiant de la tâche est dans le **fragment** de
  l'URL (`…/t/#<id>`) : il n'est jamais transmis au serveur.

Le site vitrine principal reste [boutch-pages](https://github.com/ArMen56k/boutch-pages).

## Empreintes déclarées

`com.boutch.touchefait` : clé **debug** pour le développement. Ajouter l'empreinte de la clé
**release** (SHA-256, `keytool -list -v -keystore <keystore release>`) avant la publication
Play, sans retirer la debug tant qu'on développe.
