# 🏭 Data Factory MC88 - Générateur de Données Mock

**Data Factory by MC88** est un générateur de données de test professionnel et léger qui fonctionne entièrement côté client (dans le navigateur). Il permet de créer des jeux de données réalistes et personnalisés pour tester des applications, pratiquer le nettoyage de données, créer des démonstrations ou alimenter des bases de données de développement.

---

## 📋 Prérequis

1. Un navigateur web moderne (Chrome, Firefox, Edge, Safari, Brave, Opera)
2. Aucune connexion Internet requise après le chargement initial de la page
3. Aucune installation de logiciel nécessaire

---

## 🚀 Guide d'installation complet

### Étape 1 : Télécharger le fichier

1. Téléchargez le fichier `index.html` sur votre ordinateur
2. Placez-le dans un dossier de votre choix (par exemple : `C:\DataFactory\` ou `~/Documents/DataFactory/`)

### Étape 2 : Lancer l'application

**Méthode simple (recommandée) :**
- Double-cliquez simplement sur le fichier `index.html`
- L'application s'ouvrira automatiquement dans votre navigateur par défaut

**Méthode alternative (pour les développeurs) :**
- Ouvrez votre éditeur de code (VS Code, Sublime Text, etc.)
- Ouvrez le dossier contenant `index.html`
- Utilisez l'extension "Live Server" ou similaire pour lancer un serveur local
- Accédez à `http://localhost:5500` ou `http://127.0.0.1:5500` dans votre navigateur

---

## 🎯 Guide d'utilisation détaillé

### 🔹 Étape 1 : Configurer le secteur d'activité

1. Dans la section **"Dataset Configuration"** (Configuration du jeu de données)
2. Cliquez sur le menu déroulant **"Industry Sector"** (Secteur d'activité)
3. Choisissez parmi les 8 secteurs disponibles :
   - 🛒 **Retail & E-commerce** : Commandes, produits, clients
   - 💳 **Banking & Finance** : Transactions, comptes, statuts
   - 🏥 **Healthcare** : Patients, diagnostics, médecins
   - ✈️ **Aviation & Flights** : Vols, passagers, compagnies aériennes
   - 🚚 **Logistics & Shipping** : Expéditions, expéditeurs, destinataires
   - 📚 **Education** : Étudiants, cours, notes
   - 👥 **HR & Recruitment** : Employés, départements, salaires
   - 🪪 **Personal Profiles** : Profils personnels complets

### 🔹 Étape 2 : Choisir la culture des noms

1. Cliquez sur le menu déroulant **"Name Culture"** (Culture des noms)
2. Sélectionnez parmi 9 cultures disponibles :
   - **Arabic** (Moyen-Orient) : Noms arabes, villes du Golfe, formats de téléphone arabes
   - **French** (Europe) : Noms français, villes françaises, formats de téléphone français
   - **English** (Global) : Noms anglais, villes internationales
   - **Indian** : Noms indiens, villes indiennes
   - **Canadian** : Noms canadiens, villes canadiennes
   - **Australian** : Noms australiens, villes australiennes
   - **South African** : Noms sud-africains, villes sud-africaines
   - **German** : Noms allemands, villes allemandes
   - **Spanish** : Noms espagnols, villes espagnoles

### 🔹 Étape 3 : Définir le nombre de lignes

1. Dans le champ **"Row Count"** (Nombre de lignes)
2. Saisissez manuellement un nombre (entre 1 et 50 000)
3. Ou utilisez les boutons rapides :
   - **50** : Petit échantillon
   - **200** : Échantillon moyen
   - **500** : Taille standard (défaut)
   - **2K** : 2 000 lignes
   - **5K** : 5 000 lignes
   - **15K** : 15 000 lignes
   - **50K** : 50 000 lignes (maximum)

### 🔹 Étape 4 : Configurer la graine (Seed) - Optionnel

1. Dans le champ **"Seed (optional)"** (Graine optionnelle)
2. Saisissez n'importe quel nombre ou texte
3. **Important** : La même graine + les mêmes paramètres = jeu de données identique à chaque fois
4. Laissez vide pour obtenir un jeu de données aléatoire à chaque génération
5. Utile pour :
   - Reproduire des bugs
   - Faire des démonstrations cohérentes
   - Partager des jeux de données exacts avec des collègues

### 🔹 Étape 5 : Activer le mode "Données sales" (Messy Data)

1. Cochez la case **"Generate messy data"** (Générer des données sales)
2. Utilisez le curseur pour définir le pourcentage de "saleté" (5% à 80%)
3. Les types de "saleté" injectés :
   - **Valeurs nulles** (NULL) : Cellules vides
   - **Fautes de frappe** : Caractères inversés dans les chaînes
   - **Dates incohérentes** : Formats de date mélangés (JJ/MM/AAAA au lieu de AAAA-MM-JJ)
   - **Valeurs aberrantes** : Nombres multipliés par 50 à 150 fois leur valeur normale
   - **Noms de colonnes irréguliers** : Majuscules, espaces, suffixes ajoutés
   - **Lignes dupliquées** : Copies de lignes existantes ajoutées

### 🔹 Étape 6 : Générer le jeu de données

1. Cliquez sur le bouton **"Generate Dataset"** (Générer le jeu de données)
2. Une barre de progression s'affichera
3. Attendez quelques secondes (dépend du nombre de lignes)
4. Le tableau de prévisualisation se mettra à jour automatiquement

---

## 📊 Prévisualisation des données

### Affichage du tableau

- Les **20 premières lignes** sont affichées dans le tableau de prévisualisation
- Les **en-têtes de colonnes** sont épinglés (sticky) pour faciliter le défilement
- Les **cellules NULL** sont affichées en gris italique
- Les **valeurs aberrantes** (outliers) sont affichées en rouge
- Le **nombre total de lignes** est affiché dans le badge en bas

### Indicateur de lignes

- Le badge **"X rows"** (X lignes) affiche le nombre total de lignes générées
- Formaté avec séparateurs de milliers (ex : 5 000 rows)

---

## 📤 Exportation des données (6 formats)

### Format CSV
1. Cliquez sur le bouton **"CSV"**
2. Le fichier sera téléchargé automatiquement
3. Compatible avec : Excel, Google Sheets, LibreOffice Calc, Python, R

### Format Excel
1. Cliquez sur le bouton **"Excel"**
2. Le fichier `.xlsx` sera généré et téléchargé
3. Compatible avec : Microsoft Excel, Google Sheets, LibreOffice Calc
4. Préserve les types de données (nombres, dates, texte)

### Format JSON
1. Cliquez sur le bouton **"JSON"**
2. Le fichier `.json` sera téléchargé
3. Format tableau d'objets JavaScript
4. Idéal pour : API, Node.js, Python, applications web

### Format SQL
1. Cliquez sur le bouton **"SQL"**
2. Le fichier `.sql` sera téléchargé
3. Contient :
   - `CREATE TABLE` avec toutes les colonnes
   - `INSERT INTO` pour chaque ligne
4. Compatible avec : MySQL, PostgreSQL, SQLite, MariaDB

### Format XML
1. Cliquez sur le bouton **"XML"**
2. Le fichier `.xml` sera téléchargé
3. Structure hiérarchique avec balises `<row>` et colonnes
4. Échappement automatique des caractères spéciaux

### Format Markdown
1. Cliquez sur le bouton **"Markdown"**
2. Le fichier `.md` sera téléchargé
3. Tableau Markdown prêt à l'emploi
4. Idéal pour : documentation, GitHub, wikis

### Format Parquet
- **Note** : Le format Parquet nécessite une bibliothèque dédiée
- Utilisez JSON ou CSV à la place pour l'instant
- Un message d'information s'affichera si vous cliquez sur ce bouton

### Copier dans le presse-papiers
1. Cliquez sur le bouton **"Copy"** (Copier)
2. Les 200 premières lignes seront copiées au format TSV (Tab-Separated Values)
3. Collez directement dans Excel, Google Sheets ou un éditeur de texte

### Aperçu complet
1. Cliquez sur le bouton **"Open Full Preview"** (Ouvrir l'aperçu complet)
2. Un nouvel onglet s'ouvrira avec le tableau complet
3. Toutes les lignes sont affichées avec défilement

---

## 🎨 Personnalisation de l'interface

### Thème sombre / clair

1. Cliquez sur l'icône **soleil/lune** dans l'en-tête
2. Le thème bascule entre sombre (défaut) et clair
3. Votre préférence est enregistrée automatiquement

### Bouton Reset (Réinitialiser)

1. Cliquez sur le bouton **"Reset"** dans l'en-tête
2. Efface toutes les préférences enregistrées
3. Restaure les valeurs par défaut :
   - Secteur : Retail
   - Culture : English
   - Lignes : 500
   - Graine : vide
   - Mode messy : désactivé
   - Thème : sombre

---

## 🛠️ Guide de dépannage (Problèmes courants)

### Problème 1 : Le bouton "Generate" ne fonctionne pas

**Cause :**
- Le nombre de lignes saisi est invalide (texte au lieu de nombre)
- Le nombre de lignes est supérieur à 50 000

**Solution :**
- Vérifiez que le champ "Row Count" contient un nombre valide
- Utilisez les boutons rapides pour définir une valeur correcte
- Assurez-vous que le nombre est entre 1 et 50 000

---

### Problème 2 : L'exportation ne télécharge rien

**Cause :**
- Aucun jeu de données n'a été généré
- Le navigateur bloque les téléchargements automatiques

**Solution :**
- Cliquez d'abord sur "Generate Dataset"
- Vérifiez les paramètres de téléchargement de votre navigateur
- Autorisez les téléchargements multiples pour ce site

---

### Problème 3 : Le fichier Excel ne s'ouvre pas

**Cause :**
- La bibliothèque SheetJS n'a pas été chargée
- Problème de connexion Internet au premier chargement

**Solution :**
- Vérifiez votre connexion Internet
- Rechargez la page (F5)
- Attendez que la page soit complètement chargée avant de générer

---

### Problème 4 : Les données générées sont identiques à chaque fois

**Cause :**
- Une graine (seed) fixe a été saisie dans le champ "Seed"

**Solution :**
- Videz le champ "Seed"
- Ou changez la valeur de la graine pour obtenir un nouveau jeu de données
- Rappel : même graine = mêmes données (c'est le comportement attendu)

---

### Problème 5 : La page est lente avec 50 000 lignes

**Cause :**
- 50 000 lignes est le maximum et peut être gourmand en ressources
- La prévisualisation n'affiche que 20 lignes, mais l'exportation traite tout

**Solution :**
- Utilisez moins de lignes pour les tests rapides
- Fermez les autres onglets gourmands en mémoire
- Attendez que la génération soit terminée avant d'exporter

---

### Problème 6 : Le mode "Messy Data" ne montre pas de différence

**Cause :**
- Le pourcentage de "saleté" est trop faible
- Le curseur est réglé sur 5%

**Solution :**
- Augmentez le pourcentage à 50% ou plus
- Vérifiez que la case "Generate messy data" est bien cochée
- Regardez le résumé qui s'affiche après la génération

---

### Problème 7 : Le bouton "Copy" ne copie rien

**Cause :**
- Le navigateur bloque l'accès au presse-papiers
- Aucun jeu de données n'a été généré

**Solution :**
- Générez d'abord un jeu de données
- Autorisez l'accès au presse-papiers dans les paramètres du navigateur
- Utilisez l'exportation CSV comme alternative

---

### Problème 8 : Les noms ne correspondent pas à la culture choisie

**Cause :**
- La culture a été changée après la génération
- Le jeu de données affiché est l'ancien

**Solution :**
- Cliquez à nouveau sur "Generate Dataset" après avoir changé la culture
- Vérifiez que la culture est bien sélectionnée avant de générer

---

## 💾 Sauvegarde des préférences

L'application enregistre automatiquement vos préférences dans le stockage local du navigateur :

- **Thème** (sombre/clair)
- **Secteur d'activité** sélectionné
- **Culture de noms** sélectionnée
- **Nombre de lignes** saisi
- **Graine** (seed) saisie

Pour effacer ces préférences :
1. Cliquez sur le bouton **"Reset"** dans l'en-tête
2. Ou videz le stockage local du navigateur
3. Ou utilisez la navigation privée/incognito

---

## 📄 Copyright

**Copyright © 2026**  
📧 mohamed005cheikh@gmail.com  
**Conçu et développé par MC88**  
**Tous droits réservés** | **All rights reserved**

---

## 🔗 Ressources externes utilisées

- **Font Awesome** : Icônes (v6.4.0)
- **Google Fonts** : Polices Plus Jakarta Sans, Space Grotesk, JetBrains Mono
- **SheetJS** : Bibliothèque d'exportation Excel (xlsx 0.20.1)

---

## 📝 Notes techniques

- L'application fonctionne 100% côté client (aucun serveur requis)
- Les données sont générées localement dans le navigateur
- Aucune donnée n'est envoyée sur Internet
- Le générateur de nombres aléatoires utilise l'algorithme **mulberry32**
- La graine (seed) est hachée avec un algorithme personnalisé
- Les données sont reproductibles avec la même graine
- La prévisualisation est limitée à 20 lignes pour les performances
- L'exportation gère l'intégralité du jeu de données
