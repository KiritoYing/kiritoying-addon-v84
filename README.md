# 🇫🇷 AlloCiné Stremio Addon

Addon Stremio qui intègre vos listes d'envies de films et séries AlloCiné directement dans votre interface Stremio, avec navigation par genres et tri automatique par note spectateur.

## 🚀 Installation

Ajoutez cet addon à Stremio en utilisant le lien manifest :

```
https://kiritoying.github.io/allocine-stremio-addon/manifest.json
```

## 📋 Fonctionnalités

- ✅ **Accès direct** à vos envies AlloCiné sur Stremio  
- ✅ **Tri automatique** par meilleure note spectateur
- ✅ **Navigation rapide** par genres (Action, Drame, Films Courts...)
- ✅ **Catalogues personnalisés** films et séries avec affiches françaises
- ✅ **Interface française** complète et intuitive

## 🎯 Comment ça fonctionne

### 🤖 **Génération automatique**

Cet addon est généré via un **script Python** utilisant **Chrome WebDriver** pour scraper automatiquement les listes d'envies AlloCiné. Le script :

- **Se connecte** à un profil AlloCiné spécifique
- **Parcourt** toutes les pages de films/séries en "envie de voir"
- **Extrait** les métadonnées (titre, année, réalisateur, acteurs)
- **Enrichit** les données via l'API TMDB pour obtenir les IDs IMDb
- **Génère** les catalogues JSON compatibles Stremio
- **Organise** automatiquement par genres (Action, Drame, Films Courts, etc.)

### 🔒 **Contenu actuel**

⚠️ **Important** : Pour l'instant, cet addon contient uniquement **les listes d'envies du profil AlloCiné de KiritoYing** car c'est un projet personnel/privé.

Le script n'est pas public car il nécessite :
- Configuration spécifique de Chrome WebDriver
- Gestion des cookies AlloCiné
- Clés API TMDB personnelles
- Optimisations pour éviter la détection anti-bot

### 🎬 **Contenu disponible**

- **~650+ films** de la wishlist AlloCiné de KiritoYing
- **~120+ séries** de la wishlist AlloCiné de KiritoYing
- **Navigation par genres** : Action, Animation, Comédie, Crime, Documentaire, Drame, Familial, Films Courts, Guerre, Histoire, Horreur, Musique, Mystère, Romance, Science-Fiction, Thriller, Téléfilm, Western
- **Tri automatique** par note spectateur (les mieux notés en premier)

## 🔧 Architecture technique

### **Structure des catalogues**

```
catalog/
├── movie/
│   ├── films_envies.json           # Catalogue principal films
│   └── films_envies/
│       ├── genre=Action.json       # Films par genre
│       ├── genre=Drame.json
│       └── genre=Films Courts.json
└── series/
    ├── series_envies.json          # Catalogue principal séries  
    └── series_envies/
        ├── genre=Animation.json    # Séries par genre
        └── genre=Crime.json
```

### **Enrichissement des métadonnées**

Chaque film/série contient :
- **Titre français** et **titre original**
- **Année de sortie** précise
- **IMDb ID** (quand disponible)
- **Réalisateur/Créateur** et **acteurs principaux**
- **Note spectateur** AlloCiné pour le tri
- **Posters** et **backgrounds** haute qualité via TMDB
- **Genres** détaillés avec catégorie spéciale "Films Courts"

## 🎪 Utilisation

1. **Installer l'addon** dans Stremio avec l'URL du manifest
2. **Parcourir les catalogues** "🎬 Films - Envies Allociné" et "📺 Séries - Envies Allociné"
3. **Filtrer par genre** via le menu déroulant
4. **Cliquer sur un titre** pour voir les détails complets
5. **Lancer le contenu** avec vos addons de streaming habituels

### **Genres disponibles**

**Films** : Action, Animation, Aventure, Comédie, Crime, Documentaire, Drame, Familial, Films Courts, Guerre, Histoire, Horreur, Musique, Mystère, Romance, Science-Fiction, Thriller, Téléfilm, Western

**Séries** : Animation, Comédie, Crime, Documentaire, Drame, Familial, Mystère, Western

## 🔮 Évolutions futures possibles

- **Multi-profils** : Support de plusieurs comptes AlloCiné
- **Mise à jour automatique** : Synchronisation périodique
- **Configuration** : Choix des genres à afficher
- **Recherche** : Intégration moteur de recherche Stremio

---

**Créé par KiritoYing** | Données **AlloCiné** | API **TMDB** | Compatible **Stremio**
