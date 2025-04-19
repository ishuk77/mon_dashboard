# 📊 Dashboard Épidémiologique – Analyse DHIS2

Ce projet en Python automatise tout le processus de traitement, d’analyse et de visualisation des données épidémiologiques collectées depuis **DHIS2**, afin de produire un **dashboard interactif** et des **indicateurs clés de surveillance**.

---

## 🧱 Structure du projet

```
mon_dashboard/
├── data/
│   ├── brutes/                       # Données brutes importées depuis DHIS2
│   ├── netoyes/                      # Données nettoyées
│   └── surveillance_epi_data_nettoye.xlsx
├── scripts/
│   ├── importation.py               # Importation et enregistrement des données DHIS2
│   ├── nettoyage.py                 # Nettoyage et mise en forme des données
│   ├── taux_attaque.py              # Analyse : taux d’attaque, résumé, tableaux
│   └── dashboard_epidemio.py        # Génération de cartes, graphiques et dashboard HTML
├── html/                            # Fichiers HTML de visualisation générés
├── intervalle/                      # Autres éléments web si nécessaires
├── main.py                          # Point d'entrée pour exécuter tout le pipeline
├── requirements.txt                 # Liste des bibliothèques nécessaires
└── README.md                        # Documentation du projet
```

---

## ⚙️ Étapes du pipeline

| Étape | Script | Description |
|------|--------|-------------|
| 1️⃣ | `importation.py` | Récupération automatique des données du DHIS2 |
| 2️⃣ | `nettoyage.py` | Nettoyage, normalisation et structuration des données |
| 3️⃣ | `taux_attaque.py` | Calcul des indicateurs clés (taux d'attaque, létalité, etc.) |
| 4️⃣ | `dashboard_epidemio.py` | Visualisation des données avec graphiques et cartes |

---

## ▶️ Exécution rapide

```bash
python main.py
```

💡 Ce fichier exécute automatiquement l'ensemble du processus : import, nettoyage, analyse, dashboard.

---

## 📦 Installation des dépendances

1. Crée un environnement virtuel (recommandé) :

```bash
python -m venv venv
```

2. Active-le :

- Windows : `venv\Scripts\activate`
- macOS/Linux : `source venv/bin/activate`

3. Installe les bibliothèques nécessaires :

```bash
pip install -r requirements.txt
```

---

## 🛠 Technologies utilisées

- **Pandas** – Traitement de données
- **Openpyxl** – Lecture/écriture Excel
- **Plotly / Matplotlib** – Visualisation interactive et statique
- **Folium** – Cartes interactives
- **Dash / Flask** *(si utilisé pour dashboard web)*

---

## 📂 Données

Les fichiers de données sont stockés dans :
- `data/brutes/` → données DHIS2 originales
- `data/netoyes/` → données nettoyées pour analyses
- `html/` → visualisations exportées (cartes, graphiques, dashboards)

---

## 👤 Auteur

**Shukuru Kalere-wa-Kabumba Israël**  
📧 Email : ishukuru@gmail.com  
📱 Téléphone : +243 970 955 989  

---

## 📌 À venir

- Export PDF automatique des rapports
- Connexion directe API DHIS2
- Intégration avec Tableau de bord Web (en ligne)

---
