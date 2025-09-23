# 🇫🇷 AlloCiné Stremio Addon

Ajoute vos listes d'envies de films et séries AlloCiné à Stremio avec navigation par genres et tri automatique par note spectateur.

## 🚀 Installation

Ajoutez cet addon à Stremio en utilisant le lien :

```
https://kiritoying.github.io/allocine-stremio-addon/manifest.json
```

## 📋 Fonctionnalités

- ✅ **Accès direct** à vos envies AlloCiné sur Stremio  
- ✅ **Tri automatique** par meilleure note spectateur
- ✅ **Navigation rapide** par genres (Action, Drame, Films Courts...)
- ✅ **Catalogues personnalisés** films et séries avec affiches françaises
- ✅ **Interface française** complète et intuitive

## 🎯 Fonctionnement

L'addon synchronise automatiquement avec vos listes AlloCiné :

### 🎬 **Films** 
Ajoute automatiquement de vos envies AlloCiné dans Stremio (films & séries)

### 🎭 **Tri selon la note spectateurs AlloCiné** 
Plus populaires en premier

### 🗂️ **Filtrage par genre**
Section spéciale "Films Courts" (tous les films de moins de 1h45)

### 📺 **Affiches officielles françaises**
Interface cohérente avec le contenu français

## 🔧 Structure

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

## 🎪 Utilisation

1. **Ajouter l'addon** dans Stremio avec l'URL du manifest
2. **Parcourir vos films et séries** envies via Stremio, par genre ou popularité
3. **Cliquer sur une fiche** pour voir affiche, description, durée et note spectateur
4. **Lancer le contenu** avec vos addons de streaming habituels

---
*Addon créé par KiritoYing - Données AlloCiné*
