Database
========

L'application GeoAIVision est reliée à une base de données PostgreSQL hébergée sur un serveur Amazon (AWS).  
À chaque fois qu'une nouvelle information est renseignée, les mises à jour sont automatiquement poussées vers cette base de données.

PgAdmin
-------

Pour interagir avec la base de données, utilisez **PgAdmin** en suivant les étapes ci-dessous :

1. **Ouvrir PgAdmin**  
   .. image:: pgadmin.jpg  
       

2. **Cliquer sur "Add Server"**  
   .. image:: server.jpg  
        

3. **Configurer les informations de connexion**  
   La page suivante s'ouvre, où vous pouvez renseigner les informations de connexion.  
   .. image:: connect.jpg  
       

4. **Cliquer sur "Save"**  
   .. image:: connects.jpg  
       

5. **Installation de l'extension PostGIS**  
   PostgreSQL gère les données géographiques via l'extension PostGIS. Le processus d'installation de cette extension est illustré ci-dessous :  
   .. image:: extens.jpg  
       

La base de données **hackaton_2024** a été codée en SQL. Elle contient les tables suivantes :  
`polygones`, `zones`, `fusions`, `modifications`, `suppressions`, `créations`, `utilisateurs`, et `divisions`.

Informations sur les tables
---------------------------

Voici un aperçu des principales tables de la base de données et de leur rôle :

===============   ===========================================================================
Nom de la table    Description
===============   ===========================================================================
**zone**               Les informations sur les données shapefiles et les rasters.
**polygones**          Les informations sur les polygones.
**utilisateurs**       Les informations sur les utilisateurs ou agents cartographes.
**creations**          Les nouveaux polygones créés par les utilisateurs.
**modifications**      Les modifications apportées aux polygones existants.
**suppressions**       Les polygones supprimés par les utilisateurs.
**fusions**            Les informations sur les fusions de polygones.
**divisions**          Les informations sur les divisions de polygones.
===============   ===========================================================================

