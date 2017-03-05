### Quoi:

une application online/offline pour acquérir de nouvelles données d'observation biologiques lors d'un BioBlitz avec
- Traduction automatique en [Darwin Core](http://rs.tdwg.org/dwc/) 
- Intégration des informations manquantes via des sites OpenSource (OpenTree of Life, Open Street Map, Catalogue of Life, etc.)
- Exportation vers une Base de Données
- Filtrage avec l'outil DarwinCore Validator du [GBIF](www.gbif.org)
- Exportation et publications des données vers le [GBIF](www.gbif.org)
- Configuation/Paramétrage des espèces déjà présentes sur les lieux via [GBIF](www.gbif.org) et/ou l'[INPN](https://inpn.mnhn.fr/accueil/index) pour une restriction et optimisation des ajouts d’information présente/manquante
- 3 niveaux de récupération d'information: débutant / intermédiaire / confirmé

NB: 
- 1) Il s'agit d'un outil de récupération de données pour BioBlitz et non de visualisation cartographique 
- 2) Définition BioBlitz: Un BioBlitz est une étude sur une portion bien précise de terrain, où un groupe de scientifiques et/ou de bénévoles mènent un inventaire biologique intensif pendant un temps court (24 heures ou 48 heures). L'objectif est d'identifier et de répertorier toutes les espèces d'organismes vivants présents dans une zone donnée. (Source: Wikipédia, consulté le 5 mars 2017)
- 3) [GBIF](www.gbif.org) (Global Biodiversity Information Facility) : publication et visualisation des données de biodiversité en accès libre
- 4) [Darwin Core](http://rs.tdwg.org/dwc/)  : (standard international de description pour les champs biologiques)
- 5) liens utiles: [HackPad OpenBioBlitz](https://hackpad.com/OpenBioBlitz-jVIIVR11rac)  et [l'arborescence des interfaces utilisateur/DarwinCore](https://framindmap.org/c/maps/320935/) (produits lors la Nuit du Code Citoyen à Rennes, le 3-4-5 mars). 

### Comment:

Deux interfaces offline (Utlisateurs et DarwinCore) échangent avec une API reliée à une Base de Données en ligne.
Avant d'être exportées vers le GBIF, les données sont filtrées par l'outil du GBIF DarwinCore Validator.

- 1) définissez la zone géographique et la durée de l'action: paramétrage de l'API géographique via Open Street Map
- 2) définissez le niveau de compétence des utilisateurs: configuration des information DarwinCore à rentrer
- 3) identifiez la typologie et méthodologie du BioBlitz (Bio Blitz sur oiseaux / toute forme de vie / de zone géographique ...) 

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


![](https://framindmap.org/c/maps/321124/edit)

<iframe style="width:600px;height:400px;border: 1px solid black" src="https://framindmap.org/c/maps/321124/embed?zoom=1"> </iframe>
