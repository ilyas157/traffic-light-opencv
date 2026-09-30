# Détection de feux de signalisation par vision classique

Détection et reconnaissance de l'état (rouge / vert) de feux de signalisation sans deep learning, uniquement avec OpenCV. 
Projet de traitement d'images, CY Tech, 2025.

**Pipeline :** segmentation couleur en HSV → nettoyage morphologique → filtrage des blobs lumineux par circularité → détection du boîtier (rectangles sombres filtrés par surface et ratio) → association blob / boîtier.

Interface Streamlit pour analyser les images et ajuster les paramètres en direct.

![Aperçu](streamlit_screenshots/screenshot_1.png)

**Stack :** Python · OpenCV · NumPy · Streamlit
## Installation

Suivez ces étapes pour configurer le projet sur votre machine :

1.  **Récupérer le projet**
    Téléchargez ou clonez les fichiers dans votre dossier de travail.

2.  **Ouvrez un terminal dans le dossier du projet et exécutez** :

    * **Sous Windows :**
        ```
        python -m venv venv
        .\venv\Scripts\activate
        ```

    * **Sous macOS / Linux :**
        ```
        python3 -m venv venv 
        
        source venv/bin/activate
        ```

3.  **Installer les dépendances**
    ```
    pip install opencv-python-headless numpy streamlit
    ```
4.  **Préparer les images**
    Créez un dossier nommé `image/` à la racine du projet et placez-y vos photos de test .

##  Lancement

Pour démarrer l'application,lancez :

```
streamlit run main.py
 ```
