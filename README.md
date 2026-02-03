# 📊 EUS Data Collection & Statistics System

[English](#english) | [Français](#français)

---

## <a name="français"></a>🇫🇷 Version Française

### 📝 Description

Système web standalone pour la collecte et l'analyse statistique des données de procédures d'échoendoscopie (EUS - Endoscopic Ultrasound). Cette application permet de saisir les informations détaillées des patients, de gérer une base de données locale et de générer automatiquement des statistiques et graphiques professionnels.

### ✨ Fonctionnalités principales

#### 1️⃣ **Saisie de données patient**
- Formulaire complet avec 11 sections structurées :
  - 🆔 Identité du patient
  - 🎯 Indication principale pour EUS
  - 📋 Antécédents médicaux
  - 🌡️ Signes généraux
  - 🔍 Signes fonctionnels
  - 🔬 Investigations avant EUS
  - 📍 Résultats EUS
  - ⚕️ Détails de la procédure
  - 🔬 Diagnostic et résultat
  - ⚠️ Complications
  - 📅 Suivi

- Tous les champs sont **optionnels** pour une flexibilité maximale
- Interface intuitive avec types de champs adaptés (texte, nombre, date, radio, checkbox, textarea)

#### 2️⃣ **Gestion des patients**
- 👥 Liste de tous les patients enregistrés
- ✏️ Modification des fiches patients existantes
- 🗑️ Suppression de patients
- 📥 Export des données au format JSON
- 📤 Import de données JSON

#### 3️⃣ **Statistiques et visualisations**

**4 indicateurs clés :**
- Nombre total de patients
- Taux de succès technique
- Taux d'échantillon adéquat
- Taux de complications

**8 graphiques interactifs (Chart.js) :**
1. 📊 Répartition par genre (diagramme en anneau)
2. 📊 Répartition par âge (histogramme)
3. 📊 Indications principales pour EUS (barres horizontales)
4. 📊 Type de procédure FNA vs FNB (camembert)
5. 📊 Calibre d'aiguille utilisé (diagramme en anneau)
6. 📊 Adéquation de l'échantillon (histogramme)
7. 📊 Distribution de la taille des lésions (histogramme)
8. 📊 Complications immédiates (camembert)

#### 4️⃣ **Système multilingue**
- 🇫🇷 Français
- 🇬🇧 Anglais
- Toggle simple en haut à droite
- Sauvegarde automatique de la préférence linguistique

### 🚀 Installation et utilisation

#### Prérequis
Aucun ! Il s'agit d'un fichier HTML standalone.

#### Démarrage rapide
1. Téléchargez le fichier `eus_data_collection.html`
2. Ouvrez-le dans votre navigateur web (Chrome, Firefox, Safari, Edge)
3. Commencez à saisir vos données !

#### Pas d'installation requise
- ✅ Aucun serveur nécessaire
- ✅ Aucune base de données à configurer
- ✅ Aucune dépendance externe (sauf Chart.js chargé via CDN)
- ✅ Fonctionne entièrement hors ligne (après le premier chargement)

### 💾 Stockage des données

#### Stockage local
Les données sont automatiquement sauvegardées dans le **localStorage** de votre navigateur :
- Persistance automatique à chaque enregistrement
- Données disponibles même après fermeture du navigateur
- Pas de limite pratique pour un usage médical standard

#### Export/Import
- **Export** : Téléchargez toutes vos données au format JSON
- **Import** : Restaurez vos données à partir d'un fichier JSON
- Idéal pour :
  - Sauvegardes de sécurité
  - Transfert entre ordinateurs
  - Archivage de projets
  - Partage de données anonymisées

### 📊 Calculs statistiques

Le système calcule automatiquement :

1. **Taux de succès technique** = (Procédures sans difficulté technique) / (Total de procédures) × 100

2. **Taux d'échantillon adéquat** = (Échantillons adéquats) / (Total d'échantillons) × 100

3. **Taux de complications** = (Cas avec complications) / (Total de cas) × 100

4. **Distributions** : Genre, âge, indications, types de procédures, calibres d'aiguilles, etc.

### 🔒 Sécurité et confidentialité

- ✅ **Données 100% locales** : Aucune transmission vers un serveur externe
- ✅ **Pas de compte requis** : Aucune authentification nécessaire
- ✅ **Contrôle total** : Vous gérez vos propres données
- ⚠️ **Important** : Effectuez régulièrement des exports pour sauvegarder vos données

### 📱 Compatibilité

- ✅ Desktop (Windows, macOS, Linux)
- ✅ Tablettes
- ✅ Smartphones
- ✅ Design responsive adaptatif

**Navigateurs supportés :**
- Chrome / Edge (recommandé)
- Firefox
- Safari
- Opera

### 🎨 Personnalisation

Le code est facilement modifiable si vous souhaitez :
- Ajouter de nouveaux champs au formulaire
- Modifier les graphiques
- Changer les couleurs et le design
- Ajouter d'autres langues
- Personnaliser les calculs statistiques

### 📄 Structure du fichier

```
eus_data_collection.html
├── Styles CSS (intégrés)
│   ├── Design moderne avec dégradés
│   ├── Responsive
│   └── Animations
├── HTML
│   ├── Header avec toggle de langue
│   ├── 3 onglets (Formulaire, Patients, Statistiques)
│   └── Formulaire complet
└── JavaScript (intégré)
    ├── Gestion des données (localStorage)
    ├── Système de traduction
    ├── Génération de graphiques (Chart.js)
    └── Export/Import JSON
```

### 🐛 Résolution de problèmes

**Les données ont disparu !**
- Vérifiez que vous utilisez le même navigateur
- Les données sont liées au domaine/fichier local
- Restaurez à partir d'un export JSON si disponible

**Les graphiques ne s'affichent pas**
- Vérifiez votre connexion Internet (pour charger Chart.js)
- Assurez-vous d'avoir au moins un patient enregistré

**L'export ne fonctionne pas**
- Vérifiez les autorisations de téléchargement de votre navigateur
- Essayez avec un autre navigateur

### 📞 Support

Pour toute question ou amélioration, contactez l'équipe de développement.

### 📜 Licence

Ce projet est fourni "tel quel" pour un usage médical et de recherche.

---

## <a name="english"></a>🇬🇧 English Version

### 📝 Description

Standalone web system for collecting and statistically analyzing Endoscopic Ultrasound (EUS) procedure data. This application allows you to enter detailed patient information, manage a local database, and automatically generate professional statistics and charts.

### ✨ Main Features

#### 1️⃣ **Patient Data Entry**
- Complete form with 11 structured sections:
  - 🆔 Patient identity
  - 🎯 Main indication for EUS
  - 📋 Medical history
  - 🌡️ General signs
  - 🔍 Functional signs
  - 🔬 Investigations before EUS
  - 📍 EUS findings
  - ⚕️ Procedure details
  - 🔬 Diagnosis & outcome
  - ⚠️ Complications
  - 📅 Follow-up

- All fields are **optional** for maximum flexibility
- Intuitive interface with appropriate field types (text, number, date, radio, checkbox, textarea)

#### 2️⃣ **Patient Management**
- 👥 List of all registered patients
- ✏️ Edit existing patient records
- 🗑️ Delete patients
- 📥 Export data in JSON format
- 📤 Import JSON data

#### 3️⃣ **Statistics and Visualizations**

**4 Key Indicators:**
- Total number of patients
- Technical success rate
- Adequate sample rate
- Complication rate

**8 Interactive Charts (Chart.js):**
1. 📊 Gender distribution (doughnut chart)
2. 📊 Age distribution (histogram)
3. 📊 Main indications for EUS (horizontal bars)
4. 📊 Procedure type FNA vs FNB (pie chart)
5. 📊 Needle gauge used (doughnut chart)
6. 📊 Sample adequacy (histogram)
7. 📊 Lesion size distribution (histogram)
8. 📊 Immediate complications (pie chart)

#### 4️⃣ **Multilingual System**
- 🇫🇷 French
- 🇬🇧 English
- Simple toggle in top right
- Automatic language preference saving

### 🚀 Installation and Usage

#### Prerequisites
None! This is a standalone HTML file.

#### Quick Start
1. Download the `eus_data_collection.html` file
2. Open it in your web browser (Chrome, Firefox, Safari, Edge)
3. Start entering your data!

#### No Installation Required
- ✅ No server needed
- ✅ No database to configure
- ✅ No external dependencies (except Chart.js loaded via CDN)
- ✅ Works entirely offline (after first load)

### 💾 Data Storage

#### Local Storage
Data is automatically saved in your browser's **localStorage**:
- Automatic persistence with each save
- Data available even after closing browser
- No practical limit for standard medical use

#### Export/Import
- **Export**: Download all your data in JSON format
- **Import**: Restore your data from a JSON file
- Ideal for:
  - Security backups
  - Transfer between computers
  - Project archiving
  - Sharing anonymized data

### 📊 Statistical Calculations

The system automatically calculates:

1. **Technical success rate** = (Procedures without technical difficulty) / (Total procedures) × 100

2. **Adequate sample rate** = (Adequate samples) / (Total samples) × 100

3. **Complication rate** = (Cases with complications) / (Total cases) × 100

4. **Distributions**: Gender, age, indications, procedure types, needle gauges, etc.

### 🔒 Security and Privacy

- ✅ **100% local data**: No transmission to external servers
- ✅ **No account required**: No authentication needed
- ✅ **Full control**: You manage your own data
- ⚠️ **Important**: Regularly export to backup your data

### 📱 Compatibility

- ✅ Desktop (Windows, macOS, Linux)
- ✅ Tablets
- ✅ Smartphones
- ✅ Adaptive responsive design

**Supported Browsers:**
- Chrome / Edge (recommended)
- Firefox
- Safari
- Opera

### 🎨 Customization

The code is easily modifiable if you want to:
- Add new form fields
- Modify charts
- Change colors and design
- Add other languages
- Customize statistical calculations

### 📄 File Structure

```
eus_data_collection.html
├── CSS Styles (embedded)
│   ├── Modern design with gradients
│   ├── Responsive
│   └── Animations
├── HTML
│   ├── Header with language toggle
│   ├── 3 tabs (Form, Patients, Statistics)
│   └── Complete form
└── JavaScript (embedded)
    ├── Data management (localStorage)
    ├── Translation system
    ├── Chart generation (Chart.js)
    └── JSON Export/Import
```

### 🐛 Troubleshooting

**Data disappeared!**
- Check you're using the same browser
- Data is tied to the domain/local file
- Restore from a JSON export if available

**Charts not displaying**
- Check your Internet connection (to load Chart.js)
- Make sure you have at least one patient registered

**Export not working**
- Check your browser's download permissions
- Try with another browser

### 📞 Support

For any questions or improvements, contact the development team.

### 📜 License

This project is provided "as is" for medical and research use.

---

## 🔧 Technical Details

### Technologies Used
- **HTML5** - Structure
- **CSS3** - Styling with gradients and animations
- **JavaScript (Vanilla)** - Logic and interactivity
- **Chart.js 4.x** - Data visualization
- **LocalStorage API** - Data persistence

### Data Format (JSON)
```json
{
  "fullName": "John Doe",
  "medicalRecordNumber": "12345",
  "age": 45,
  "gender": "Male",
  "lesionLocation": "Mediastinum",
  "lesionSize": 25.5,
  "procedureType": "FNA",
  "needleGauge": "22G",
  "sampleAdequacy": "Adequate",
  ...
}
```

### Browser Storage
- **Key**: `eusPatients` (array of patient objects)
- **Language Key**: `eusLanguage` (string: 'fr' or 'en')

---

**Version**: 1.0  
**Last Updated**: February 2025  
**Developed for**: Medical research and EUS data analysis
