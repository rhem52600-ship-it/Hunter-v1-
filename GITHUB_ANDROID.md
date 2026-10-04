# HUNTER V1 — compilation Android depuis un smartphone

## Méthode
1. Crée un compte sur GitHub.
2. Crée un nouveau dépôt, par exemple `HUNTER-V1`.
3. Depuis le navigateur Android, ouvre le dépôt puis **Add file > Upload files**.
4. Envoie **le contenu de ce dossier** (pas le ZIP lui-même), en conservant notamment `.github/workflows/build-apk.yml`.
5. Valide le commit sur la branche `main`.
6. Ouvre l'onglet **Actions** du dépôt.
7. Ouvre **Build HUNTER APK** et attends la fin du workflow.
8. Ouvre le workflow terminé et va dans **Artifacts**.
9. Télécharge `HUNTER-V1-debug-apk`.
10. Décompresse l'archive téléchargée : elle contient `app-debug.apk`.
11. Ouvre `app-debug.apk` sur Android pour installer HUNTER.

## Si le workflow ne démarre pas
Dans **Actions > Build HUNTER APK**, utilise **Run workflow**.

## Important
Cette version est un APK de test/debug. Pour publier sur Google Play, il faudra ensuite créer une clé de signature et produire une version release signée.
