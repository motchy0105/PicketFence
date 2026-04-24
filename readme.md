# 📊 Picket Fence Analyzer – MLC standard/HD

Application permettant l’analyse automatique des tests **Picket Fence** à partir d’images DICOM, avec génération de rapports PDF et Excel.

---

## 🚀 Fonctionnalités

- Analyse automatique d’images DICOM (Picket Fence)
- Détection du type de faisceau (X6, X6FFF, X18)
- Calcul des écarts MLC (gap, positions)
- Validation automatique (OK / NOK)
- Génération de :
  - PDF d’analyse
  - PDF tableau
  - Excel détaillé
- Fusion automatique des rapports

---

## ▶️ Utilisation

1. Lancer l’exécutable :
- PickAndFence_Novalis.exe pour un MLC HD
- PickAndFence_Gemini.exe pour un MLC standard


2. Sélectionner une image DICOM

3. Laisser l’application :
- détecter le faisceau
- analyser les lames MLC
- générer les rapports (lors de la fermeture de l'application)

---

## 📄 Sorties

Pour chaque analyse :

- `*.xlsx` → données détaillées
- `*_fusion.pdf` → rapport final

---

## ⚙️ Configuration

Les fichiers :
- picket_ref_positions_novalis.json
- picket_ref_positions_gemini.json
![json](/images/.png)

permettent de définir :

- Positions théoriques (correspondant à la moyenne de la position CAX de la fente souhaitée, cf. exemple)
- Gap nominal (correspondant à la moyenne des largeurs des différentes fentes, cf. exemple)
- Plages d’angles
- Énergies
![Exemple tableau](/images/exemple.png)
---

## ⚠️ Notes

- L’image doit être au format DICOM
- Tolérance actuelle : ±1 mm
- La plage de l’angle du gantry doit être inscrite dans le fichier .json

---

## 👨‍🔬 Auteur

Motchy SALEH  
Physicien médical – CHR Metz-Thionville / CRAN

---

## 📬 Feedback

Les retours sont les bienvenus pour améliorer l’outil (bugs)👍 
Mail : motchy.saleh@chr-metz-thionville.fr
