# Faire un scipt PowerShell qui va permettre l'utilisation du remoteApp

##  Aperçu
Le project à pour but d'aider les utilisateur à utiliser le **remotteApp**. La seule tâche qui vont le rester à faire manuellement sera de modifier leur fichier.rdp **Aller voir le Quoi modifier**


---

##  Objectifs
- Permettre d'appliquer les modification avec intune
- Permettre l'utilisation de plusieurs application avec le moins d'action humaine possible
- Ensure service reliability
- Validate deployment automatically

---

##  Techno utilisé 
- PowerShell
- Éditeur du Registre
- RDP

---

##  Que fait le script ?

Le script effectue les actions suivantes :

1. Vérifie que le compte utilisé est celui de l'utilisateur et non adm*
2. S'assure d'utiliser les bon path même si le path contient une version
3. S'assure que les clés ne se recrée pas pour rien
4. Valide que l'utilisateur à l'application sinon ne crée aucune clé

---

##  Quoi modifier

### éditer le fichier.rdp avec notepad et modifier les lignes suivante

1. Modify remoteapplicationmode:i:0  to  remoteapplicationmode:i:1

2. Add remoteapplicationprogram:s:Notepad

3. Add disableremoteappcapscheck:i:1

4. Add alternate shell:s:rdpinit.exe


