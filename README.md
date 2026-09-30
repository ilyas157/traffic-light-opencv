# Détection de Feux de Signalisation

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