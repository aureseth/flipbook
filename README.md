<a name="readme-top"></a>
<!--
*** Thanks for using Document My Project. (https://github.com/luisvent/document_my_project) 
*** If you have a suggestion that would make this better, please fork  
*** the repo and create a pull request or simply open an issue.
*** Don't forget to give the project a star!
-->

<p align="center"><a href="https://github.com/luisvent/document_my_project/graphs/contributors"><img src="https://img.shields.io/github/contributors/luisvent/document_my_project.svg?style=for-the-badge" alt="Contributors"></a>
        <a href="https://github.com/luisvent/document_my_project/network/members"><img src="https://img.shields.io/github/forks/luisvent/document_my_project.svg?style=for-the-badge" alt="Forks"></a>
        <a href="https://github.com/luisvent/document_my_project/stargazers"><img src="https://img.shields.io/github/stars/luisvent/document_my_project.svg?style=for-the-badge" alt="Stargazers"></a>
        <a href="https://github.com/luisvent/document_my_project/issues"><img src="https://img.shields.io/github/issues/luisvent/document_my_project.svg?style=for-the-badge" alt="Issues"></a></p><br/>


<div align="center">

<a href="" target="_blank" title="Go to  website">
<img width="196px" alt="Flipbook" src="../assets/images/icon.png">
</a>

# Flipbook

Création rapide d'un fichier Flipbook

</div>


<div align="center"><h4><a href="#-table-of-contents">️Table of Contents</a> • <a href="#-about-the-project">ℹ️ About the Project</a> • <a href="#-showcase">🏞 Showcase</a> • <a href="#-features">⭐️ Features</a> • <a href="#-stack-tech">🛠 Stack Tech</a> • <a href="#-setup">⚙ ️Setup</a> • <a href="#configuration-settings-ini-">Configuration (settings.ini)</a> • <a href="#d-pannage">Dépannage</a> • <a href="#-acknowledgements">🏆 Acknowledgements</a> • <a href="#-contributing">👏🏻 Contributing</a> • <a href="#-about-the-author">👨🏻‍ About the Author</a> • <a href="#-license">📖 License</a></h4></div>

<p align="center"><img src="../assets/images/dmp_1.png" alt="Main Image"/></p>

## ️Table of Contents
 <details>
<summary>Open Contents</summary>

- [Flipbook](#flipbook)
  - [ℹ️ About the Project](#-about-the-project)
  - [🏞 Showcase](#-showcase)
  - [⭐️ Features](#-features)
  - [🛠 Stack Tech](#-stack-tech)
  - [⚙ ️Setup](#-setup)
    - [Installation](#installation)
  - [Configuration (settings.ini)](#configuration-settingsini)
  - [Dépannage](#dpannage)
    - [Usage](#usage)
  - [🏆 Acknowledgements](#-acknowledgements)
  - [👏🏻 Contributing](#-contributing)
    - [Ways to Contribute](#ways-to-contribute)
    - [Contribution Instructions](#contribution-instructions)
    - [Contributors](#contributors)
  - [👨🏻‍ About the Author](#-about-the-author)
  - [📖 License](#-license)
</details>

## ℹ️ About the Project

Répond au besoin d'intégration à certain site d'une lecture de fichier pdf en flipbook, qui est cet effet "livre". 



## 🏞 Showcase

 <center>

<table>
<tr>
<td><a href=""><img width="320" src=""></a></td>
<td></td>
</tr>
</table>

</center>

## ⭐️ Features

1. **Découpage d'images**

Transforme un PDF en autant d'images qui le compose

2. **Création du Flipbook**

Facilitation de création du Flipbool



## 🛠 Stack Tech
- [![Angular][Angular-badge]][Angular-url] - A front-end web application framework

[Angular-badge]: https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular
[Angular-url]: }
- [![NgRx][NgRx-badge]][NgRx-url] - Angular state management based on Redux

[NgRx-badge]: https://img.shields.io/badge/NgRx-B7116E?style=for-the-badge&logo=ngrx
[NgRx-url]: }
- [![Tailwind CSS][Tailwind CSS-badge]][Tailwind CSS-url] - Utility-first CSS framework

[Tailwind CSS-badge]: https://img.shields.io/badge/Tailwind%20CSS-38B2AC?style=for-the-badge&logo=tailwindcss
[Tailwind CSS-url]: }
- [![TypeScript][TypeScript-badge]][TypeScript-url] - A strict syntactical superset of JavaScript

[TypeScript-badge]: https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript
[TypeScript-url]: }


## ⚙ ️Setup

### Installation

To install this project, follow these steps:

1. Pré-requis

Python 3.8+:**  Assurez-vous que Python 3.8 ou une version supérieure est installé et ajouté au PATH de votre système. Vous pouvez le vérifier en ouvrant une invite de commandes et en tapant `python --version`.
2.  **curl:**  L'utilitaire `curl` doit être installé et accessible dans le PATH.  Vous pouvez le télécharger depuis [https://curl.se/windows/](https://curl.se/windows/).  Testez l'installation avec `curl --version`.
3.  **Droits d'écriture:**  L'utilisateur exécutant le script doit avoir les droits d'écriture dans le répertoire où le script est placé.
4.  **Accès à SharePoint Online:** Vous devez disposer d'un site SharePoint Online et connaître son URL complète (par exemple, `https://votreentreprise.sharepoint.com/sites/votresite`).

2. Structure des dossiers : 

Flipbook/
├── config/
│   └── settings.ini  <- Fichier de configuration (URL SharePoint, qualité image)
├── fait/             <- Les PDF traités sont déplacés ici
├── flipbook_generator.py  <- Script Python principal
├── html_cible/       <- Les fichiers HTML générés sont placés ici
├── logs/             <- (créé par le script)
├── pdf_cible/        <- Les images extraites des PDF sont placées ici (sous-dossiers par PDF)
├── pdf_source/       <- Placez les fichiers PDF à convertir ici
└── venv/             <- Environnement virtuel Python (créé par le script)
deploy_log.txt    <- Fichier journal du déploiement

3. ## Installation et Utilisation

1.  **Téléchargez les fichiers:** Placez tous les fichiers (le script `.bat`, `flipbook_generator.py`, et le dossier `config`) dans un dossier, par exemple, `C:\Flipbook`.  *Il est crucial que le script batch et le dossier `Flipbook` soient dans le même répertoire.*

2.  **Placez les PDF:**  Copiez les fichiers PDF que vous souhaitez convertir dans le dossier `Flipbook\pdf_source`.

3.  **Exécutez le script:** Double-cliquez sur le fichier `.bat`.  Le script effectuera les actions suivantes :

    *   Création d'un environnement virtuel Python (`venv`).
    *   Installation des dépendances Python (PyMuPDF et Pillow).
    *   Vérification de la version de Python et de la présence de `curl`.
    *   Demande de l'URL de votre site SharePoint Online (si ce n'est pas déjà configuré).  *Cette URL sera stockée dans `config\settings.ini`.*
    *   Création de l'arborescence des dossiers (si elle n'existe pas déjà).
    *   Génération du script Python `flipbook_generator.py` (si il n'existe pas déjà).
    *   Exécution du script Python pour convertir les PDF.
    *  Enregistrement des actions, et des erreurs potentielles, dans le fichier `deploy_log.txt`

4.  **Résultat:**
    *   Les images de chaque page de chaque PDF seront stockées dans un sous-dossier (nommé d'après le PDF) dans `Flipbook\pdf_cible`.  Par exemple, `Flipbook\pdf_cible\mon_pdf\page_1.jpg`.
    *   Un fichier HTML pour chaque PDF sera créé dans `Flipbook\html_cible`.  Par exemple, `Flipbook\html_cible\mon_pdf.html`.
    *   Les fichiers PDF originaux seront déplacés vers le dossier `Flipbook\fait`.

5.  **Intégration SharePoint:**
    *   Copiez le contenu des dossiers `pdf_cible` et `html_cible` vers votre site SharePoint Online.  Vous pouvez les placer dans une bibliothèque de documents, par exemple.
    *   Pour afficher le flipbook, vous pouvez utiliser un composant WebPart "Visionneuse de fichiers" et le lier au fichier HTML correspondant, ou bien utiliser le web part "Embed" avec l'URL du fichier HTML généré. Ou bien, vous pouvez créer une page SharePoint et y intégrer le flipbook en utilisant l'URL du fichier HTML.  L'important est que les images (dossier `pdf_cible`) et le fichier HTML soient accessibles depuis SharePoint.

## Configuration (settings.ini)

Le fichier `config\settings.ini` contient les paramètres suivants :

*   `sharepoint_base_url`: L'URL de base de votre site SharePoint Online.  Exemple: `https://votreentreprise.sharepoint.com/sites/votresite`.
*   `image_quality`: La qualité des images JPEG générées (valeur entre 0 et 100, 85 par défaut).  Une valeur plus élevée signifie une meilleure qualité, mais aussi une taille de fichier plus grande.

## Dépannage

*   **Erreurs lors de l'exécution:** Consultez le fichier `deploy_log.txt` pour les messages d'erreur détaillés.
*   **Python non trouvé:** Assurez-vous que Python est installé et que le chemin d'accès à l'exécutable Python est ajouté à la variable d'environnement PATH de votre système.
*   **curl non trouvé:**  Installez `curl` et ajoutez son répertoire `bin` au PATH.
*   **Problèmes de droits d'écriture:** Exécutez le script en tant qu'administrateur.
*    **URL SharePoint Invalide:** Vérifiez l'URL fournie, et qu'elle commence bien par `https://`



### Usage

After installation, you can use the project by following these steps:

1. Open the project directory in your code editor

2. Run `npm run start` to start the development server



## 🏆 Acknowledgements

- [Mistral]() - https://mistral.ai/
- [Gemini]() - https://gemini.google.com/


## 👏🏻 Contributing

We welcome contributions from the community! If you would like to contribute to this project, please follow the guidelines below.

### Ways to Contribute

- Report bugs or issues by opening a new issue on our GitHub repository.
- Suggest new features or improvements by opening a new issue on our GitHub repository.
- Contribute code by forking the repository, making changes, and submitting a pull request.

### Contribution Instructions

1. Fork the repository.
2. Create a new branch for your feature or bug fix: `git checkout -b my-feature-branch`.
3. Make the necessary changes and commit them: `git commit -am 'Add my new feature'`.
4. Push your branch to your forked repository: `git push origin my-feature-branch`.
5. Open a pull request against the main repository, describing the changes you made and why they should be merged.


## 👨🏻‍ About the Author

**Aurélien Rodier**

This project was created by Aurélien Rodier. 


## 📖 License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).


<p align="right"><a href="#readme-top">Top ⬆️</a></p>

---
 <div align="center">Built with ❤️ with <a href="https://github.com/luisvent/document_my_project">Document My Project</a></div>

