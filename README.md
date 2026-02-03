# 📊 EUS Data Collection & Statistics System

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
