# TP

Réalisation d'une application de météo

## API Meteo

L'API vous donnant les données météo est la suivante : 
===> https://openweathermap.org/api
(doc) ===> https://openweathermap.org/api/one-call-3

**Astuce : pour la réalisation des appels API, utiliser le ```fetch()``` dans un ```componentDidMount()```**


## Design appplication


RDV sur Figma pour récupérer les maquettes
===> https://www.figma.com/community/file/1171124278675784716/Weather-Meter-App

**Attention : n'utiliser QUE les 2 maquettes de droite, dans la page "Screen"**


## Fonctionnalités 

1. Arrivée sur la page d'accueil de votre application : on doit voir la barre de recherche ET la liste de toutes les villes déjà recherchées
2. La barre de recherche doit permettre d'ajouter une ville à la liste
3. Le click sur une ville (de la page d'accueil) doit vous permettre d'afficher la page de détail de la ville en question


## Étapes de réalisation

1. Create-react-app
2. Mise en place du router pour les 2 routes des 2 types de page
3. Mise en place des pages & des composants en dur (commencer par les props)
4. Basculer les props en "State" => pour permettre le rafraichissement régulier de l'APP
5. **Option 1** (plus facile) ===> Mettre en place un ```tick``` (cf doc) pour MAJ les données toutes les 15 secondes
**Option 2** (moins facile) ===> Se servir du ```useEffect()``` pour MAJ les données toutes les 15 secondes


### Listing des PAGES && Composants à réaliser

- **ACCUEIL**
  - Titre
  - Barre de recherche
  - Ville(s)
    - Température
    - Image
    - Latitude/Longitude
    - Nom_ville, Nom_pays
- **DETAIL_DUNE_VILLE**
  - Header
    - Nom_ville
    - Température + tendance
  - Qualité_de_lair
    - Titre
    - Nombre (progress_bar)
  - Indice_UV
    - Titre
    - Nombre
  - Lever_du_soleil
    - heure_de_lever
    - heure_de_coucher
  - Vent
    - Vitesse
    - Direction
  - Hydrométrie
    - derniere_heure
    - prochaines_24_heures
  - Taux_humidité
    - pourcentage
  - Température_ressentie
    - nombre
    - comparaison_temperature_reelle

