# AGENTS.md — Instructions projet

## Contexte du projet
Site web personnel d'un chercheur, redige en francais, base sur Quarto (`.qmd`) avec un dossier `teaching/` (cours, syllabus, slides) et une generation statique.
Le contenu est majoritairement en francais et contient beaucoup d'accents.

## Regles de travail (prioritaires)
1. **Encodage**
   - Ne jamais casser les accents : **preserver l'encodage UTF-8**.
   - **Interdit** : ecrire des fichiers via `Set-Content` ou `Out-File` sans forcer UTF-8.
   - **Autorise** : `apply_patch` (prefere) ou ecriture explicite en UTF-8 (sans BOM) si necessaire.
2. **Modifs de fichiers**
   - Preferer les modifications ciblees plutot que les remplacements globaux.
   - Toujours relire les caracteres accentues apres modification.
3. **Quarto**
   - Ne pas modifier la structure des pages sans raison claire.
   - Garder la structure des sections (titres, blocs, HTML embed) identique sauf demande explicite.

## Environnements disponibles
- **Python 3.12.7 (Conda: base)**
  `C:\Users\Admin\anaconda3\python.exe`
- **Python 3.10.18 (Conda: pyllm)**
  `C:\Users\Admin\anaconda3\envs\pyllm\python.exe`
- **R 4.4.1 (System)**
  `C:\Program Files\R\R-4.4.1\bin\x64\R.exe`

## Bonnes pratiques specifiques
- Si un changement touche plusieurs fichiers texte, **demander confirmation** avant d'appliquer.
- Mentionner clairement chaque fichier modifie et le but de la modification.
- Ne pas supprimer/renommer des fichiers sans demande explicite.
