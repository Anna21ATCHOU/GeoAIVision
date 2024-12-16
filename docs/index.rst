.. GeoAIVision documentation master file, created by
   sphinx-quickstart on Fri Dec  6 09:40:36 2024.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Bienvenue dans la documentation de GeoAIVision!
===============================================

GeoAIVision est une application mobile conçue pour traiter des fichiers shapefile. Son objectif est de permettre à l'utilisateur, tel qu'un agent cartographe, de modifier la structure des polygones d'un shapefile et d'ajouter des informations pertinentes (maison habitée ou pas, nombre de personnes, etc.) concernant ces éléments géographiques.

.. note::
   La version la plus aboutie de l'application se trouve dans la branche `final_app` de ce dépôt GitHub : 
   `https://github.com/Mafieuu/SenMapEditor/tree/final_app` dans le dossier `_finalapp`. Elle comporte :
   
   - Une page de connexion
   - Un bouton pour se déconnecter
   - Un bouton pour sauvegarder les modifications
   - Les fonctionnalités de création et de suppression de polygones.

   De plus, elle utilise une base de données locale **SQLite**, similaire à celle présente sur AWS. Cela permet d'abandonner les fichiers GeoJSON au profit de **SQLite** pour faciliter le transfert des données modifiées par l'utilisateur de son appareil mobile vers le cloud.

   Malheureusement, cette version comporte un bug qui empêche l'utilisateur de se connecter. Nous tentons de résoudre ce problème, mais en raison des contraintes de temps et des exigences académiques de notre école, nous n'avons pas encore réussi. Par conséquent, nous nous rabattons sur une version moins sophistiquée de notre application, située dans la branche **main** dans le dossier `senmapeditor`.

.. toctree::
   :maxdepth: 2
   :caption: Contents:

   Inscription
   Connexion
   Selection
   Questionnaire
   Database

Indices and tables
==================

* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
