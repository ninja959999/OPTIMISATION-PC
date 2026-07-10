# 🛠️ Ninja Gaming — Boîte à outils PC

Trois petits outils faits maison pour nettoyer, organiser et optimiser un PC Windows gaming.

---

## 📦 1. Explorateur Disque

Application graphique (Python/Tkinter) pour visualiser ce qui prend de la place sur le disque, naviguer dans les dossiers, chercher, et supprimer en toute sécurité.

**Fonctionnalités**
- Scan avec barre de progression en temps réel
- Tri automatique par taille décroissante avec barre visuelle par élément
- Navigation en double-clic (rentrer/sortir des dossiers)
- Barre de recherche pour filtrer
- Classification automatique : 🎮 Jeux, ⚙️ Programmes, 🎬 Média, 📄 Documents, 🧹 Caches (safe à vider), ⚠️ Système Windows
- Avertissement spécial avant suppression d'un dossier système important
- Ouverture directe dans l'explorateur Windows

**Prérequis** : Python 3 (aucune dépendance externe, Tkinter est inclus).

**Utilisation**
```bash
python explorateur_disque_v2.py
```
ou double-clic sur `lancer_explorateur_v2.bat`.

[⬇️ Télécharger explorateur-disque.zip](explorateur-disque.zip)

---

## 🗂️ 2. Organiseur de fichiers

Script Python qui range automatiquement le dossier Downloads par catégorie, en se basant sur des mots-clés dans le nom (marche aussi pour les dossiers extraits, jeux, assets) et sur l'extension en fallback.

**Catégories par défaut** : Wallpapers, Assets_GameDev, Logiciels, Patches_Mods, Jeux, Images, Vidéos, Documents, Archives, Code...

Les mots-clés et catégories sont personnalisables directement en haut du script (`KEYWORD_CATEGORIES`, `EXTENSION_CATEGORIES`).

**Prérequis** : Python 3 (aucune dépendance externe).

**Utilisation**
```bash
python file_organizer.py
```
ou double-clic sur `organiser_fichiers.bat`.

[⬇️ Télécharger organiser-fichiers.zip](organiser-fichiers.zip)

---

## 🎮 3. Mode Gaming (optimisation Valorant)

Script PowerShell qui bascule le PC en mode "Performance" avant de lancer un jeu (pensé pour Valorant), et permet de tout restaurer après.

**Ce qu'il fait**
- Ferme les applications gourmandes en arrière-plan (Steam, Discord, navigateurs, launchers...) — liste personnalisable
- Passe le plan d'alimentation Windows sur "Performances élevées"
- Mode restauration pour revenir à la config normale après la session de jeu

**Utilisation**
```powershell
.\game_perf_mode.ps1          # active le mode perf
.\game_perf_mode.ps1 -Restore # revient au mode normal
```
Ou plus simple : double-clic sur `Activer_Mode_Gaming.bat` (active) et `Restaurer_Mode_Normal.bat` (restaure).

⚠️ Nécessite d'autoriser l'exécution de scripts PowerShell (géré automatiquement par le `.bat` via `-ExecutionPolicy Bypass`).

[⬇️ Télécharger mode-gaming.zip](mode-gaming.zip)

---

*Fait par Ninja Gaming.*
