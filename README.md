_OpenBioBlitz est un projet initié et développé lors de la première édition de [la Nuit du Code Citoyen](https://codecitoyen.github.io/villes/rennes.html) le 4-5 mars 2017 à Rennes (Bretagne)_

### Quoi:

une application online/offline pour acquérir de nouvelles données d'observation biologiques lors d'un BioBlitz avec
- Traduction automatique en [Darwin Core](http://rs.tdwg.org/dwc/) 
- Intégration des informations manquantes via des sites OpenSource (OpenTree of Life, Open Street Map, Catalogue of Life, etc.)
- Exportation vers une Base de Données
- Filtrage avec l'outil DarwinCore Validator du [GBIF](www.gbif.org)
- Exportation et publications des données vers le [GBIF](www.gbif.org)
- Configuration/Paramétrage des espèces déjà présentes sur les lieux via [GBIF](www.gbif.org) et/ou l'[INPN](https://inpn.mnhn.fr/accueil/index) pour une restriction et optimisation des ajouts d’informations présentes et manquantes
- 3 niveaux de récupération d'information: débutant / intermédiaire / confirmé

### Comment:

Deux interfaces online/offline (utlisateurs et DarwinCore) échangent avec une API reliée à une Base de Données en ligne.
Avant d'être exportées vers le GBIF, les données sont filtrées par l'outil du [GBIF DarwinCore Validator](http://tools.gbif.org/dwca-validator).

### Solutions techniques possibles :

**Forms**

Different level (beginner, intermediate, expert)
Remember that information could be automatically completed later (kingdom, etc.)
Different kind of box (box, textbox, combobox, listbox, list, button, etc.)
Different kind of inputs (images, geo-ref, text, etc.)
Create prelist to help user

**Portable app**

Think about a complete offline apps form need to charge forms informations before going outline. => need also a small replication of the database or a specific format (json) that will be used by the api during upload on database.
Upload data when go back online (or at the end of bioblitz)

**API**

Interface between database and apps (webform and portable apps)

**Database**

Portable
SQL or not
Simple
Uniform and sharable think in terms of DWC archive and data exportation

**Web app**

Prepare forms
Project access (ACL)
Basic data visualisation => not the main objective

