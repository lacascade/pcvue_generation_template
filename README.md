# pcvue_generation_template
Dispositif permettant de générer des écrans PCVUE à partir d'une description.

## Fichiers

Cet utilitaire est composé de 2 fichiers :
* un fichier archive au format .zip contenant l'arborescence des dossiers nécessaires pour créer les écrans de pcvue
* un fichier excel contenant les macros vba pour importer des variables de factory io, générer un dossier PCVUE, créer un fichier d'import pour les variables

## Notice d'utilisation
Dans le répertoire Usr de votre installation de PCVUE, dézipper l'archive
Vérifier que l'arborescence est celle-ci : PCVUE/Usr/template_projet/..., le dossier template_projet doit se trouver sous Usr

Dans Factory IO version 2.4, se rendre dans la console et exécuter la ligne suivante : drivers.export_mapping('mon_export_factory'), ceci va générer un fichier csv (Exports mapping of scene tags and driver I/O points) dans le dossier Documents\Factory IO\
Ensuite cliquer sur le bouton "Importer fichier", afin d'importer les variables dans la feuille "Import"

Dans la feuille "Projet" :
* renseigner le chemin de votre installation PCVUE
* donner un nom à votre projet
* lister les écrans, leur donner un nom, une description et un modèle (il en existe 2 accueil et écran)

Cliquer sur le bouton "Générer le projet"

Exporter la liste des variables pour les importer dans PCVUE à l'aide du bouton "Exporter"

Vous pouvez lancer PCVUE et choisir votre projet. Aller ensuite dans l'import PCVUE et sélectionner l'import générique.
Les variables importées seront disponibles dans le dossier Import.