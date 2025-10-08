# Exercice Intermédiaire 3
## Commande utilisé
### - `journalctl -u ssh --since "24 hours ago"`
<img width="1004" height="308" alt="image" src="https://github.com/user-attachments/assets/0ec320c2-f1ac-4ec5-a73d-036e37717f8c" />

##### Recupere toute les logs ssh des dernière 24h

### - `journalctl -u ssh --since "24 hours ago" | grep "Failed password"`
##### Filtre les logs pour garder seulement les connexions ratées

### - `journalctl -u ssh --since "24 hours ago" | grep "Failed password" > sshd_failed_logins.txt`
##### Sauvegarde le résultat qui a étais filtrer dans un fichier

### Une fois terminer vous pouvez voir les logs contenant Failed password avec la commande `cat sshd_failed_logins.txt`
<img width="1186" height="151" alt="image" src="https://github.com/user-attachments/assets/de1e3c53-2561-4a35-90c9-6358e42a8afd" />

