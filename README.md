# 🧰 Poker Tools

Ce dépôt contient les outils d’orchestration pour le projet **Poker**, notamment le fichier `docker-compose.yml` permettant de lancer les services **API** et **Front-end** en local.

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
- Clonez dans un premier temps 'poker-tools' puis au sein de ce dossier, clonez `poker-front` et `Poker-API`

### 2. Clonage des dépôts

```bash
git clone https://github.com/MDS-poker-project/poker-tools.git
git clone https://github.com/MDS-poker-project/poker-front.git
git clone https://github.com/MDS-poker-project/Poker-API.git
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
Ibragimova Maria
Boutrois Benjamin