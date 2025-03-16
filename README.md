# LinkedIn Job Scraper

## 📌 Description
Ce projet est un **scraper Python** permettant d'extraire des offres d'emploi depuis **LinkedIn** et de classifier les intitulés de poste en différentes spécialités techniques. Il stocke les résultats dans un fichier CSV et élimine les doublons.

## 🚀 Fonctionnalités
- **Scraping des offres d'emploi** depuis LinkedIn
- **Normalisation** des titres de poste
- **Classification automatique** en fonction de mots-clés (Développement Web, BI & Big Data, Cloud, Embarqué, etc.)
- **Élimination des doublons** dans les fichiers CSV

## 🛠️ Installation
### Prérequis
- Python 3.x installé
- Bibliothèques nécessaires :

```bash
pip install requests beautifulsoup4 numpy scikit-learn
```

## 📜 Utilisation
1. **Lancer le script** :
   ```bash
   python scraper.py
   ```
2. Les résultats seront enregistrés dans `linkedin-jobs.csv`.
3. Les doublons seront supprimés et les données finales enregistrées dans `linkedin-jobs-noduplicates.csv`.

## 📁 Structure du projet
```
/linkedIn-job-scraper
├── scraper.py
├── linkedin-jobs.csv
├── linkedin-jobs-noduplicates.csv
├── requirements.txt
└── README.md
```

## 📝 Explication des modules principaux
- `normalize_string(string)`: Nettoie et normalise les chaînes de caractères.
- `determine_speciality(title)`: Analyse le titre du poste et l'associe à une spécialité.
- `linkedin_scraper(url, page_number, writer)`: Scrape les offres et les enregistre dans un CSV.
- `remove_duplicates(input_file, output_file)`: Supprime les doublons et assigne une spécialité à chaque offre.
- `main()`: Point d'entrée du script.

## 🤝 Contribution
Les contributions sont les bienvenues ! Si vous souhaitez ajouter des fonctionnalités ou améliorer le code, n'hésitez pas à soumettre une pull request.

## 📜 Licence
Ce projet est sous licence MIT. Consultez le fichier `LICENSE` pour plus d'informations.

🚀 **Happy Scraping !**

