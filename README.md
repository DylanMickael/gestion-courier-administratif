# AdminMail - Système de Gestion de Courrier Intelligent

Un système intelligent de numérisation, génération et d'archivage de courriers administratifs. Ce projet utilise **FastAPI** pour le backend modulaire, **LlamaIndex (LlamaExtract)** pour l'OCR structuré, **Groq AI** pour la génération de contenu, et propose une interface **Vanilla JS** premium avec un sélecteur de thèmes.

## 🚀 Fonctionnalités Clés

- **OCR Intelligent (Image & PDF)** : Extraction automatique de données structurées depuis des documents scannés ou des fichiers PDF via LlamaExtract.
- **Génération IA** : Création de courriers officiels personnalisés via l'IA Groq (Llama 3.3), exportables en PDF.
- **Thèmes Personnalisables** : Mode "Full Dark" ou Mode Clair avec une palette élégante Noir/Blanc/Or.
- **Gestion Complète (Historique)** : Enregistrement, consultation (OCR preview), recherche et suppression des courriers.
- **Export PDF** : Génération de documents PDF professionnels respectant les standards administratifs.

## 🛠️ Structure du Projet

```text
gestion-courrier-administratif/
├── backend/            # Backend FastAPI Modulaire
│   ├── app/
│   │   ├── api/        # Endpoints (Routes)
│   │   ├── core/       # Configuration & Schémas
│   │   ├── models/     # Modèles Pydantic
│   │   ├── services/   # Logique OCR & IA Creation
│   │   └── utils/      # Générateur PDF
│   ├── assets/         # Logos & Ressources
│   ├── main.py         # Point d'entrée de l'application
│   └── requirements.txt
├── frontend/           # Interface Web (HTML/CSS/JS)
│   ├── css/            # Styles (Dual Theme + Gold Accents)
│   └── js/             # Logique UI & Intégration PDF.js
└── README.md
```

## ⚙️ Installation

### 1. Prérequis
- Python 3.9+
- Clés API : [LlamaIndex](https://cloud.llamaindex.ai/) & [Groq](https://console.groq.com/)

### 2. Configuration du Backend
1. Naviguer dans le dossier `backend/`.
2. Créer et activer l'environnement virtuel :
   ```bash
   virtualenv venv
   .\venv\Scripts\activate
   ```
3. Installer les dépendances :
   ```bash
   pip install -r requirements.txt
   ```
4. Créer un fichier `.env` :
   ```env
   LLAMA_CLOUD_API_KEY=votre_cle_llama
   GROQ_API_KEY=votre_cle_groq
   ```

### 3. Lancement
```bash
python main.py
```
L'application est accessible sur **`http://localhost:8000`**.

## 📖 Utilisation

1. **Entrée** : Importez une photo ou un PDF pour extraire les données.
2. **Sortie** : Décrivez votre besoin et laissez l'IA rédiger le courrier.
3. **Historique** : Gérez vos archives et téléchargez vos exports PDF.

---
*Optimisé pour l'efficacité administrative.*
