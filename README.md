# TP_Note_traitement_du_signal_2025


🔧 Étape 1 — Installer la dernière version de Python

Aller sur :
👉 https://www.python.org/downloads/

Télécharger la dernière version stable (Python 3.12.x ou +).

Pendant l'installation :
✅ Cocher Add Python to PATH
Puis cliquer sur Install Now.

Vérifier l’installation :

python --version


ou

python3 --version

🖥️ Étape 2 — Installer Visual Studio Code

Télécharger VS Code :
👉 https://code.visualstudio.com/

Installer normalement.

🧩 Étape 3 — Installer les extensions Python dans VS Code

VS Code → CTRL + SHIFT + X → rechercher :

Python (Microsoft)

Pylance (Microsoft)

Jupyter (optionnel pour notebooks)

Installer les trois.

🧪 Étape 4 — Créer un environnement virtuel

Dans le dossier du projet :

python -m venv venv


Activer l’environnement :

Windows
venv\Scripts\activate

Mac / Linux
source venv/bin/activate


Vous devez voir :

(venv)

🔎 Étape 5 — Sélectionner l’interpréteur Python dans VS Code

CTRL + SHIFT + P

Taper : Python: Select Interpreter

Choisir :

Mac / Linux :

.venv/bin/python


Windows :

venv\Scripts\python.exe

🎵 Étape 6 — Installer les bibliothèques pour traitement audio
Bibliothèques principales :
pip install numpy scipy matplotlib librosa soundfile scikit-learn pandas

Pour les modèles avancés (deep learning, spectrogrammes) :
pip install torch torchvision torchaudio

🚀 Structure recommandée du projet
projet_audio/
│── README.md
│── requirements.txt
│── main.py
│── src/
│     ├── preprocessing.py
│     ├── extract_features.py
│     ├── train_model.py
│     ├── evaluate.py
│── data/
│     ├── raw/
│     ├── processed/
│── models/
│── notebooks/
