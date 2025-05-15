# 🧰 Poker Tools

Ce dépôt contient les outils d’orchestration pour le projet **Poker**, notamment le fichier `docker-compose.yml` permettant de lancer les services **API** et **Front-end** en local.

## Description

Ce projet est une application web (front, back, db) de poker. Il s'inscrit dans le cadre de notre formation chez MyDigitalSchool ayant pour objectif de créer une application web complète.

- Front : **React**
- Back : **Nest**
- Database : **Sqlite**
- Documentation : **Swagger**
- Tests : **Jest & Swagger**

## 🗂 Structure du projet

L’arborescence du projet est la suivante (les trois dépôts sont clonés dans un même dossier parent) :

```
    /poker-tools/
    ├── poker-api/
    ├── poker-front/
    └── docker-compose.yml
```


## 🚀 Lancement du projet

### 1. Pré-requis

- [Docker](https://www.docker.com/) installé et opérationnel

### 2. Clonage des dépôts

## Méthode 1

Clonez dans un premier temps 'poker-tools' :
```bash
git clone https://github.com/MDS-poker-project/poker-tools.git
```

Ensuite, naviguez vers ce dossier :
```bash
cd poker-tools
```

Puis clonez `poker-front` et `Poker-API` grâce aux sous modules :

```bash
git submodule update --init --recursive
```

## Méthode 2

Clonez tous les repos en même temps

```bash
git clone --recurse-submodules https://github.com/MDS-poker-project/poker-tools.git
```

### 3. Lancer les services

Depuis le dossier `poker-tools`, exécuter :

```bash
docker-compose up -d
```

Cela lance les conteneurs `poker-front` et `Poker-API`

⚠️ Le conteneur 'Poker-API' peut être très long à servir l'api (~5min sur Windows)

### 4. Arrêter les services

Depuis le dossier `poker-tools`, exécuter :

```bash
docker-compose down
```

## Auteurs
- Ibragimova Maria
- Boutrois Benjamin